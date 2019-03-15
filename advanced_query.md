---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creating an advanced monitoring query (Beta)
{: #creating-an-advanced-monitoring-query-beta}

In the {{site.data.keyword.cloud}}, you can use Grafana, an open source analytics and visualization platform to monitor, search, analyze, and visualize your metrics in various graphs, for example charts and tables. You can use Grafana to perform advanced analytical tasks.
{:shortdesc}

If you use Grafana, you can use the dashboard to create graphs using the metric query.
1. [Navigate to the Grafana dashboard](/docs/services/cloud-monitoring/grafana?topic=cloud-monitoring-navigating_grafana#navigating_grafana).
2. Select the domain `account` and a user account with an IBMid linked to the bare metal device.
3. Use this format to create your queries.
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. Here are the available metric types:
<table>
   <CAPTION>Table 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Type</th>
     <th>Units</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>bytes</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>bytes</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>bytes</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>bytes</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>bytes/second</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>bytes/second</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>operations/second</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>operations/second</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>latency in milliseconds per operation</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>latency in milliseconds per operation</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` or `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>bytes/second</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` or `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>bytes/second</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` or `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>number</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` or `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>number</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` or `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>number</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` or `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>number</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>This metric isn't available for all devices.</td>
       <td>degrees Celsius</td>
     </tr>
   </TBODY>
   </table>

For more information, see [Configuring a metric query in Grafana](/docs/services/cloud-monitoring/grafana?topic=cloud-monitoring-define_query#define_query).
