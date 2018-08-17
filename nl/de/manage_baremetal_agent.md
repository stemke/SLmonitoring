---
copyright:
  years: 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta) verwalten

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent erfasst Metrikdaten von dem Gerät, auf dem der Service installiert ist, und sendet diese an den Metrikspeicher. Über den Metrikspeicher stehen die Daten für die Benutzerschnittstelle für einfache Überwachungsprozesse und für Grafana für erweiterte Abfragen zur Verfügung.
Wenn Sie IBM Cloud Monitoring Service for IaaS Bare Metal Agent verwenden, führen Sie die nachfolgenden Schritte durch, um den Service für den Server anzuzeigen, zu stoppen, zu starten oder zu deinstallieren.
{:shortdesc}

<table>
   <CAPTION>Tabelle 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Gewünschte Aktion...</th>
   <th>Vorgehensweise unter Linux...</th>
     <th>Vorgehensweise unter FreeBSD...</th>
     <th>Vorgehensweise unter Windows...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Status des Service anzeigen</td>
   <td>
   Verwenden Sie den Befehl `service monitoring status`.
   </td>
     <td>
   Verwenden Sie den Befehl `service monitoring status`.
   </td>
     <td>
   Verwenden Sie den Befehl `sc.exe query monitoring`.
   </td>
   </tr>
   <tr>
   <td>Überwachungsservice stoppen</td>
   <td>
   Verwenden Sie den Befehl `service monitoring stop`.
   </td>
     <td>
   Verwenden Sie den Befehl `service monitoring stop`.
   </td>
     <td>
   Verwenden Sie den Befehl `sc.exe stop monitoring`.
   </td>
   </tr>
       <tr>
   <td>Überwachungsservice starten</td>
   <td>
   Verwenden Sie den Befehl `service monitoring start`.
   </td>
     <td>
   Verwenden Sie den Befehl `service monitoring start`.
   </td>
     <td>
   Verwenden Sie den Befehl `sc.exe start monitoring`.
   </td>
   </tr>
       <tr>
   <td>Überwachungsservice deinstallieren</td>
   <td>Geben Sie die folgenden Befehle ein:
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>Geben Sie die folgenden Befehle ein:
     <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>Führen Sie die folgenden Schritte durch:
 <ol>
       <li>Rufen Sie über die Systemsteuerung die Option zum **Deinstallieren von Programmen** auf.</li>
       <li>Wählen Sie **IBM Cloud Monitoring Agent** aus.</li>
   <li>Klicken Sie auf **Deinstallieren**.</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>



