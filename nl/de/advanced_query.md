---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Erweitere Überwachungsabfrage erstellen (Beta)

In {{site.data.keyword.cloud}} können Sie Grafana, eine Open-Source-Plattform für Analysen und Visualisierungen, verwenden, um Ihre Metriken in verschiedenen grafischen Darstellungen, beispielsweise in Diagrammen und Tabellen, zu überwachen, zu durchsuchen, zu analysieren und zu visualisieren. Mit Grafana können Sie erweiterte Analysetasks durchführen.
{:shortdesc}

Wenn Sie Grafana verwenden, können Sie mithilfe der Metrikabfrage Diagramme erstellen.
1. [Navigieren Sie zum Grafana-Dashboard](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-navigating_grafana#navigating_grafana).
2. Wählen Sie die Domäne `account` und ein Benutzerkonto mit einer IBMid aus, die mit dem Bare-Metal-Gerät verknüpft ist.
3. Verwenden Sie das folgende Format zum Erstellen der Abfragen.
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. Nachfolgend sind die verfügbaren Metriktypen aufgeführt:
<table>
   <CAPTION>Tabelle 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Typ</th>
     <th>Geräte</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>Byte</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>Byte</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>Byte</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>Byte</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>Byte/Sekunde</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>Byte/Sekunde</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>Operationen/Sekunde</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>Operationen/Sekunde</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>Latenz in Millisekunden pro Operation</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>Latenz in Millisekunden pro Operation</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` oder `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>Byte/Sekunde</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` oder `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>Byte/Sekunde</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` oder `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>Zahl</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` oder `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>Zahl</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` oder `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>Zahl</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` oder `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>Zahl</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>Diese Metrik ist nicht für alle Geräte verfügbar.</td>
       <td>Grad Celsius</td>
     </tr>
   </TBODY>
   </table>

Weitere Informationen finden Sie in [Metrikabfrage in Grafana konfigurieren](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-define_query#define_query).
