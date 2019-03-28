---

copyright:
  years: 2014, 2019
lastupdated: "2019-02-06"

keywords:

subcollection: slautoscale

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Automatische Skalierung mit Apache Brooklyn
{: #auto-scale-with-apache-brooklyn}

## Einführung

Ein Unternehmen, das täglich mehr als einer Milliarde mobilen Benutzern kritische Kundendaten bereitstellt, hat uns gebeten, die Funktionalität bereitzustellen, mit der Auto Scale-Gruppen mit Servern in einem privaten Netz erstellt werden können. Eine zentrale Anforderung war Elastizität, die ermöglicht, dass die Systeme in Reaktion auf die Anforderungen durch die Arbeitslast und die Reaktionszeit für das Benutzererlebnis in Übereinstimmung mit vordefinierten Richtlinien per Scale-up bzw. Scale-down automatisch nach oben bzw. nach unten skaliert werden.

Die automatische Skalierung basiert auf der CPU-Nutzung. Wenn die durchschnittliche CPU-Nutzung der Server in einer Gruppe den obersten Schwellenwert bzw. das Ereignis für die Auslösung überschreitet, müssen mehr Ressourcen bereitgestellt werden, d. h. es ist eine vertikale Skalierung nach oben durch Scale-up notwendig. Wenn die durchschnittliche CPU-Nutzung der Server in einer Gruppe den untersten Schwellenwert bzw. das Ereignis für die Auslösung unterschreitet, müssen die Ressourcen zurückgeschraubt werde, d. h. es ist eine vertikale Skalierung nach unten durch Scale-down notwendig. Der Kunde stellte die folgenden Anforderungen:

1. Möglichkeit zur Angabe der folgenden Parameter:
  * Ursprüngliche Anzahl von Servern in der Gruppe
  * Mindest- und Höchstanzahl von Servern in der Gruppe
  * Oberer und unterer Schwellenwert der CPU-Auslastung
  * Anzahl der zusätzlichen Server, um die bei Eintreten des Auslöserereignisses die vertikale Skalierung nach oben (Scale-up) bzw. nach unten (Scale-down) erfolgen soll
2. Integration des DNS (Domain Name System)
  * Nachdem ein Server in der Gruppe bereitgestellt worden oder per Scale-up nach oben skaliert worden und verfügbar ist, soll für ihn ein entsprechender DNS-Datensatz erstellt werden.
  * Wenn der Server im Rahmen des Scale-down entfernt wird, soll der zugehörige DNS-Datensatz ebenfalls entfernt werden.
3. Integration mit einer Lastausgleichsfunktion
  * Nachdem ein Server in der Gruppe bereitgestellt worden oder per Scale-up nach oben skaliert worden und verfügbar ist, muss der Serverdatensatz zur entsprechenden NetScaler-Lastausgleichsfunktion hinzugefügt und an die entsprechende Lastausgleichsgruppe gebunden werden.
  * Wenn der Server im Rahmen des Scale-down entfernt wird, muss die Bindung an die entsprechende Lastausgleichsgruppe aufgehoben und der Serverdatensatz aus NetScaler entfernt werden.
4. Integration von Chef
  * Nachdem ein Server in der Gruppe bereitgestellt worden oder per Scale-up nach oben skaliert worden und verfügbar ist, soll der Chef-Client ausgeführt werden und den Knoten beim Chef-Server registrieren.
  * Wenn der Server im Rahmen des Scale-down entfernt wird, sollen der Knoten und der Clientdatensatz auf dem Server vom Chef-Server entfernt werden.
5. Anforderungen für die Bereitstellung von Servern
  * Alle Server in der Gruppe sollen als VMs (virtuelle Maschinen) mit ausschließlich privaten Uplinks, 1.000 MB/s Portgeschwindigkeit und einem angegebenen privaten VLAN bereitgestellt werden.
  * Die Bereitstellung virtueller Maschinen (VMs) soll über die Standardvorlage für mehrere Platten erfolgen, die vom Kunden in {{site.data.keyword.cloud}} erstellt worden ist.
6. Betriebssystem
  * CentOS 7

Basierend auf den Anforderungen des Kunden wurde Apache Brooklyn zur Implementierung der Lösung als das Tool für die automatische Skalierung ausgewählt.

## Überblick über Apache Brooklyn

Apache Brooklyn ist ein Framework zum Modellieren, Überwachen und Verwalten von Anwendungen mittels autonomer Entwürfe. Weitere Informationen finden Sie auf der Website von [Apache Brooklyn ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://brooklyn.incubator.apache.org/){: new_window}.

### Konzepte von Apache Brooklyn

Die Dokumentation für Apache Brooklyn enthält Definitionen von Apache Brooklyn-Konzepten wie den folgenden:

* Entitäten
* Anwendung
* Konfiguration von übergeordneten Elementen und der Zugehörigkeit
* Sensoren und Effektoren
* Lebenszyklus- und Managementkontext
* Abhängige Konfiguration
* Standort und Richtlinien
* Ausführung
* Implementierung

![Abbildung 1: Lösungsdesign für Lastausgleich und automatische Skalierung](images/figure1-1.png)

`Abbildung 1: Lösungsdesign für Lastausgleich und automatische Skalierung`

### Integration von DNS, NetScaler und Chef

Apache Brooklyn stellt als Basisklasse zum Anpassen des Standorts die Klasse `brooklyn.location.jclouds.BasicJcloudsLocationCustomizer` bereit. Diese Klasse enthält Methoden, die bei der Bereitstellung von Maschinen die Erstellung zusätzlicher Parameter ermöglichen. Aktionen können ausgeführt werden, nachdem eine Maschine bereitgestellt wurde und - wenn sie storniert wurde - bevor und nachdem sie freigegeben wurde.

Wir haben eine eigene Klasse für die Standortanpassung erstellt, die die von Brooklyn bereitgestellte Klasse `brooklyn.location.jclouds.BasicJcloudsLocationCustomizer` erweitert. Im vorliegenden Beispiel wird sie als `brooklyn.location.jclouds.ProjectJcloudsLocationCustomizer` bezeichnet.

Die folgenden drei Methoden wurden außer Kraft gesetzt:

1. `public void customize(JcloudsLocation location, ComputeService computeService, TemplateOptions templateOptions)` - Diese Methode wird gestartet, bevor die Cloud-API zum Bereitstellen eines Servers aufgerufen wird. Wir haben die Fähigkeit zur Angabe von Bereitstellungseigenschaften wie `privateNetworkOnly, primaryBackendNetworkComponentVlanId, portSpeed` und anderen aktiviert.

* `public void customize(JcloudsLocation location, ComputeService computeService, JcloudsSshMachineLocation machine)` - Diese Methode wird gestartet, nachdem eine Maschine bereitgestellt und gestartet worden ist und daher alle Serverparameter wie die Server-IP-Adresse verfügbar sind. In diese Methode muss der Code zum Hinzufügen eines Servers zum DNS und zum Lastausgleich eingefügt werden. Das DNS und die REST-API für NetScaler werden verwendet, um die DNS-Datensätze zu erstellen und den Server an NetScaler zu binden. Wir haben ein von `Brooklyn, brooklyn.util.http` bereitgestelltes Paket verwendet, um REST-Aufrufe an das DNS und die NetScaler-APIs zu übergeben.

* `public void preRelease(JcloudsSshMachineLocation machine)` - Diese Methode wird beim Stornieren der Maschine gestartet, bevor der Server gestoppt wird. Hier haben wir REST-Aufrufe an das DNS und NetScaler-Datensätze hinzugefügt, um die DNS- und NetScaler-Datensätze zu entfernen und die Bindung des Servers an die NetScaler-Gruppe aufzuheben.

Es waren keine besonderen Schritte nötig, um den neuen Server mit Chef zu verbinden. Auf dem Image, das für die Bereitstellung des Servers verwendet wurde, war bereits ein Chef-Client sowie ein Startscript installiert. (Dieses Script führt den Chef-Client aus und verbindet ihn mit dem Chef-Server.) Wenn Sie möchten, können Sie die Brooklyn-Integration mit Chef verwenden, um Entwürfe zu erstellen.

Außerdem haben wir einen REST-Aufruf zum Chef-Server hinzugefügt, um die entsprechenden Client- und Knoten-Datensätze zu entfernen.

### Anwendungsentwurf

Innerhalb des Anwendungsentwurfs haben wir den Standort, die Parameter für die Erfassung von Metriken und die Eigenschaften der Server für die automatische Skalierung angepasst. Die folgenden Befehle werden zur Anpassung der einzelnen Komponenten verwendet.

    name: Group1
    location:

      jclouds:softlayer:tor01:
      customizerType: brooklyn.location.jclouds.ProjectJcloudLocationCustomizer
      privateNetworkOnly: true
      primaryBackendNetworkComponentVlanId: 12345
      portSpeed: 1000
      imageId: 123456
      dnsZoneId: 12345
      netscalerGroup: app1
      netscalerGroupPort: 8080
      netscalerUrl: http://user:password@10.10.10.10/nitro/v1/

    services:
    - type: brooklyn.entity.group.DynamicCluster
      id: cluster
      name: dynamic cluster
      initialSize: 1
      memberSpec:
        $brooklyn:entitySpec:
        name: VMinSL
        type: brooklyn.entity.basic.EmptySoftwareProcess
        brooklyn.initializers:
        - type: brooklyn.entity.software.ssh.SshCommandSensor
          brooklyn.config:
            name: server.cpucount
            command: "LANG=en_US.UTF-8 sar -u 1 1|grep Average | awk '{print 100 - $8}'"
            targetType: java.lang.Double
            period: 10s
          brooklyn.config:
            post.launch.command: "sudo apt-get install -y sysstat"

      brooklyn.enrichers:
      - type: brooklyn.enricher.basic.Aggregator
        brooklyn.config:
          enricher.sourceSensor: $brooklyn:sensor("server.cpucount")
          enricher.targetSensor: $brooklyn:sensor("server.cpucount.averaged")
          enricher.aggregating.fromMembers: true
          transformation: average
        brooklyn.policies:
        - policyType: brooklyn.policy.autoscaling.AutoScalerPolicy
        brooklyn.config:
          metric: $brooklyn:sensor("server.cpucount.averaged")
          metricLowerBound: 10
          metricUpperBound: 60
          minPoolSize: 1
          maxPoolSize: 5

### Standort

Im Abschnitt für den Standort haben wir unter anderem die folgenden Eigenschaften für die Bereitstellung angegeben:

* Ort, an dem der Server bereitgestellt werden soll (Rechenzentrum und VLAN)
* Ob der Server mit der Option 'privateNetworkOnly' bereitgestellt wird
* Image-ID der {{site.data.keyword.cloud_notm}}-Standardvorlage oder des Flex Image
* Portgeschwindigkeit

Außerdem haben wir die Zonen-ID des DNS angegeben, die von `ProjectJcloudLocationCustomizer` zum Hinzufügen und Löschen von Datensätzen in der DNS-Zone und von NetScaler-Informationen zum Binden des Servers an NetScaler sowie zum Aufheben dieser Bindung verwendet wird.

    location:

      jclouds:softlayer:tor01:
        customizerType: brooklyn.location.jclouds.ProjectJcloudLocationCustomizer
        privateNetworkOnly: true
        primaryBackendNetworkComponentVlanId: 12345
        portSpeed: 1000
        dnsZoneId: 12345
        netscalerGroup: app1
        netscalerGroupPort: 8080
        netscalerUrl: http://user:password@10.10.10.10/nitro/v1/

### Services

Im Abschnitt des Entwurfs für Services haben wir Folgendes angegeben:

* Dass eine Gruppe von Servern bereitgestellt wird
* Was Brooklyn auf jedem Server installieren sollte
* Wie die CPU-Metriken erfasst und verwendet werden sollten
* Wie die Parameter der Richtlinie für die automatische Skalierung lauten

#### Anwendungs-Spezifikation

    services:
    - type: brooklyn.entity.group.DynamicCluster #gruppe von servern
      id: cluster
      name: dynamic cluster
      initialSize: 1 #anzahl der ursprünglich in der gruppe erstellten server

#### Mitgliedsspezifikation

Der Aufruf `brooklyn.entity.basic.EmptySoftwareProcess` wurde verwendet, weil Apache Brooklyn nur Bereitstellungsserver aus einem Image benötigte und keine zusätzliche Installation oder Konfiguration erforderlich war. In diesem Abschnitt wurde auch ein Sensor (server.cpucount) angegeben, der für die Erfassung der CPU-Auslastung in regelmäßigen Abständen sorgt.

    memberSpec:
      $brooklyn:entitySpec:
      name: VMinSL
      type: brooklyn.entity.basic.EmptySoftwareProcess
      brooklyn.initializers:
      - type: brooklyn.entity.software.ssh.SshCommandSensor
        brooklyn.config:
          name: server.cpucount
          command: "LANG=en_US.UTF-8 sar -u 1 1|grep Average | awk '{print 100 - $8}'"
          targetType: java.lang.Double
          period: 10s
      brooklyn.config:
        post.launch.command: "sudo apt-get install -y sysstat"

### Metriken

Im Abschnitt des Entwurfs für Metriken werden Metriken von einzelnen Servern erfasst, deren Durchschnitt dem Sensor auf Clusterebene zugewiesen wird.

    brooklyn.enrichers:
      - type: brooklyn.enricher.basic.Aggregator
        brooklyn.config:
          enricher.sourceSensor: $me0$brooklyn:sensor("server.cpucount.averaged")
          enricher.aggregating.fromMembers: true
          transformation: average

### Richtlinien für die automatische Skalierung

In diesem Abschnitt sind die Eigenschaften der Richtlinien für die automatische Skalierung definiert:

    brooklyn.policies:
    - policyType: brooklyn.policy.autoscaling.AutoScalerPolicy
      brooklyn.config:
        metric: $brooklyn:sensor("server.cpucount.averaged")
        metricLowerBound: 10
        metricUpperBound: 60
        minPoolSize: 1
        maxPoolSize: 5
        minPeriodBetweenExecs: 10m
        resizeUpIterationIncrement: 2
        resizeUpIterationMax: 2
        resizeDownIterationIncrement: 2
        resizeDownIterationMax: 2

Nachdem die Lösung bereitgestellt wurde, konnten die Benutzer ihre Anwendungen nahtlos und automatisch vertikal per Scale-up und Scale-down zeitnah skalieren, indem sie die Systemdatensätze bei den Lastausgleichsservern, DNS-Servern und Chef registrierten bzw. deren Registrierung zurücknahmen.
