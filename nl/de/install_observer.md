---

copyright:
  years: 2018
lastupdated: "2018-04-20"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta) installieren

Damit die erweiterte Überwachung auf vorhandenen {{site.data.keyword.baremetal_short}}-Instanzen funktioniert, führen Sie nachfolgenden Schritte durch, um {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent auf Ihrem Bare-Metal-Gerät zu installieren.

## Voraussetzungen
Sie müssen mit Ihrem Bare-Metal-Gerät verbunden sein, um die Installationsprogramme herunterladen und ausführen zu können.

## Installation unter Windows

1. Laden Sie das Installationsprogramm für den IBM Cloud Monitoring-Agenten für Windows herunter. [Laden Sie Folgendes herunter: ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi){: new_window}
2. Führen Sie das Installationsprogramm auf der Zielmaschine aus.

## Installation unter Linux

1. Laden Sie das Installationsprogramm für den IBM Cloud Monitoring-Agenten für Linux herunter. [Laden Sie Folgendes herunter: ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz){: new_window}
2. Extrahieren Sie die Datei auf der Zielmaschine.
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. Führen Sie das Script 'linux_install.sh' aus.


## Installation unter FreeBSD
1. Laden Sie das Installationsprogramm für den IBM Cloud Monitoring-Agenten für FreeBSD herunter. [Laden Sie Folgendes herunter: ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz){: new_window}
2. Extrahieren Sie die Datei auf der Zielmaschine.
       `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. Führen Sie das Script 'freebsd_install.sh' aus.

## Nächste Schritte

Nach dem Ausführen der Installation schließt das System den Prozess automatisch ab. Unter Windows wird eine Nachricht mit der Bestätigung der erfolgreichen Installation oder mit Informationen zu möglichen Fehlern angezeigt.

Wenn Sie eine Firewall verwenden, müssen Sie möglicherweise angeben, dass der IBM Cloud Monitoring-Agent Daten durch diese Firewall senden darf. Der Agent verwendet Port 8090 für die abgehende HTTPS-Kommunikation. Weitere Informationen zu IP-Adressen, die Sie eventuell zulassen müssen, finden Sie in der Veröffentlichung zu den [IP-Bereichen für die Lastausgleichsfunktion](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-load-balancer-ips#load-balancer-ips).
