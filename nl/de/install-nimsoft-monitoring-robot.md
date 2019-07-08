---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Nimsoft Monitoring Robot installieren und verwalten
{: #installing-and-managing-the-nimsoft-monitoring-robot}

Damit die erweiterte Überwachung auch auf vorhandenen {{site.data.keyword.baremetal_short}}- oder {{site.data.keyword.BluVirtServers_short}}-Instanzen funktioniert, muss Nimsoft Monitoring Robot installiert sein. Mit Nimsoft Monitoring Robot kann das Überwachungsmanagementsystem mit dem Bare-Metal-Server oder virtuellen Server im privaten Netz kommunizieren. Nach der Installation von Nimsoft Monitoring Robot dauert es ca. fünf bis zehn Minuten, bis die Software in der {{site.data.keyword.cloud}}-Konsole verfügbar ist. Anhand der folgenden Schritte können Sie Nimsoft Monitoring Robot unter Windows oder Linux installieren.

## Voraussetzungen

Vor der Installation müssen die folgenden Ports zum privaten Netzwerk geöffnet sein:

* tcp/48000
* tcp/48001
* tcp/48002

Außerdem müssen die Ports tcp/48003 bis tcp/50000 für das private Netzwerk ebenfalls geöffnet sein, damit die von der API verwendete Funktionalität vollständig zur Verfügung steht. Wenn Sie diese Ports nicht öffnen, kann sich dies auf einige Überwachungsagenten auswirken. Wenn während der Konfiguration Fehler auftreten, stellen Sie sicher, dass diese Ports geöffnet sind, bevor Sie ein Ticket für die weitere Eskalation öffnen.

* **openjdk** ist für bestimmte Überwachungsagenten, wie Tomcat Monitoring Agent, erforderlich.
* Einige 64-Bit-Linux-Distributionen erfordern **glibc.i686** und **nss-softtokn-freebl.i686**.
* Das Überwachungssystem wird unter **FreeBSD** nicht unterstützt.

Falls beim Konfigurieren des Überwachungsservice durch einen Kommunikationsfehler mit Nimsoft Monitoring Robot ein Fehler auftritt, kann der Konfigurationsprozess möglicherweise aufgrund der begrenzten Konnektivität angehalten werden. Eine häufige Ursache für dieses Problem ist eine Firewall oder eine andere Sicherheitssoftware, die den Zugriff des Nimsoft-Management-Servers auf das System blockiert. Anhand der folgenden Schritte können Sie den Überwachungsservice erneut bereitstellen:

## Überwachungsagent erneut bereitstellen
{: #restarting-provisioning-of-a-monitoring-agent}

Anhand der folgenden Schritte können Sie den Überwachungsservice erneut bereitstellen:
1. Navigieren Sie zum Gerätemenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Geräten navigieren](https://test.cloud.ibm.com/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Geräte** die Option **Überwachung** aus.
3. Suchen Sie nach dem System, für das die Überwachungsfunktion konfiguriert werden soll.
4. Wählen Sie **Alle Agenten erneut bereitstellen** im Abschnitt **Erweitert** aus.
5. Wählen Sie auf der aufgerufenen Seite **** eine Überwachungsvorlage aus.
6. Klicken Sie auf **Erneut bereitstellen**.

## Installation unter Windows
{: #install-windows}

1. Besuchen Sie 'http://downloads.service.softlayer.com/nimsoft/', um die aktuelle Version von Windows Installer auf das Gerät herunterzuladen und zu installieren (Sie müssen mit dem Kunden-VPN verbunden sein).
2. Führen Sie die ausführbare Datei zu Nimsoft Monitoring Robot als Administrator aus.

## Installation unter Linux
{: #install-linux}

1. Stellen Sie über das Kunden-VPN eine Verbindung zum privaten Netz her.
2. Laden Sie die [32-Bit- ![Symbol für externen Link ](../../icons/launch-glyph.svg "Symbol für externen Link")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} oder [64-Bit-Version ![Symbol für externen Link ](../../icons/launch-glyph.svg "Symbol für externen Link ")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} des Linux-Installationsprogramms auf das Gerät herunter und installieren Sie sie. Versionen für Debian und Ubuntu sind ebenfalls im [Nimsoft Installer ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://downloads.service.softlayer.com/nimsoft/){: new_window} verfügbar.
3. Führen Sie die folgenden Befehle aus, um die Installation abzuschließen. Ersetzen Sie bei einer 64-Bit-Installation '32' durch '64'.

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Nächste Schritte

Nach dem Ausführen der Installation schließt das System den Prozess automatisch ab. Unter Windows wird eine Nachricht mit der Bestätigung der erfolgreichen Installation oder mit Informationen zu möglichen Fehlern angezeigt.

