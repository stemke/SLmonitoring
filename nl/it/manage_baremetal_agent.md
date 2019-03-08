---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestione di IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent raccoglie i dati di metrica dal dispositivo su cui è installato e li invia all'archiviazione delle metriche. Dall'archiviazione delle metriche, i dati sono disponibili per l'interfaccia utente per il monitoraggio semplice e Grafana per le query avanzate.
Se stai utilizzando IBM Cloud Monitoring Service for IaaS Bare Metal Agent, attieniti alla seguente procedura per visualizzare, arrestare, avviare o disinstallare il servizio per il tuo server.
{:shortdesc}

<table>
   <CAPTION>Tabella 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Se l'azione da intraprendere è ...</th>
   <th>Allora per Linux...</th>
     <th>Allora per FreeBSD...</th>
     <th>Allora per Windows...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Visualizzare lo stato del servizio</td>
   <td>
   Utilizza il comando `service monitoring status`
   </td>
     <td>
   Utilizza il comando `service monitoring status`
   </td>
     <td>
   Utilizza il comando `sc.exe query monitoring`
   </td>
   </tr>
   <tr>
   <td>Arrestare il servizio di monitoraggio</td>
   <td>
   Utilizza il comando `service monitoring stop`
   </td>
     <td>
   Utilizza il comando `service monitoring stop`
   </td>
     <td>
   Utilizza il comando `sc.exe stop monitoring`
   </td>
   </tr>
       <tr>
   <td>Avviare il servizio di monitoraggio</td>
   <td>
   Utilizza il comando `service monitoring start`
   </td>
     <td>
   Utilizza il comando `service monitoring start`
   </td>
     <td>
   Utilizza il comando `sc.exe start monitoring`
   </td>
   </tr>
       <tr>
   <td>Disinstallare il servizio di monitoraggio</td>
   <td>Immetti questi comandi:
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>Immetti questi comandi:
  <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>Attieniti alla seguente procedura:
 <ol>
       <li>Apri **Add or Remove Programs**.</li>
       <li>Seleziona **IBM Cloud Monitoring Agent**</li>
   <li>Fai clic su **Uninstall**.</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>
