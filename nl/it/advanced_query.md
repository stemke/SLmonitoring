---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creazione di una query di monitoraggio avanzato (Beta)

In {{site.data.keyword.cloud}}, puoi utilizzare Grafana, una piattaforma di analisi e visualizzazione open source, per monitorare, ricercare, analizzare e visualizzare le tue metriche in una varietà di grafici, ad esempio, diagrammi e tabelle. Puoi utilizzare Grafana per eseguire attività di analisi avanzate.
{:shortdesc}

Se utilizzi Grafana, puoi utilizzare il dashboard per creare grafici utilizzando la query della metrica.
1. [Vai al dashboard Grafana](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-navigating_grafana#navigating_grafana).
2. Selezionare il dominio `account` e un account utente con un ID IBM collegato al dispositivo bare metal.
3. Utilizza questo formato per creare le query.
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. Questi sono i tipi di metrica disponibili:
<table>
   <CAPTION>Tabella 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Tipo</th>
     <th>Unità</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>byte</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>byte</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>byte</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>byte</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>byte/secondo</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>byte/secondo</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>operazioni/secondo</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>operazioni/secondo</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>latenza in millisecondi per operazione</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>latenza in millisecondi per operazione</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` o `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>byte/secondo</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` o `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>byte/secondo</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` o `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>numero</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` o `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>numero</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` o `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>numero</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` o `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>numero</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>Questa metrica non è disponibile per tutti i dispositivi. </td>
       <td>gradi Celsius</td>
     </tr>
   </TBODY>
   </table>

Per ulteriori informazioni, vedi [Configuring a metric query in Grafana](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-define_query#define_query).
