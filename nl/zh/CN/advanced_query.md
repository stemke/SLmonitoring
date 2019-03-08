---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 创建高级监视查询 (Beta)

在 {{site.data.keyword.cloud}} 中，Grafana 是一种开放式源代码分析和可视化平台，可以使用它通过各种图形（例如，图表和表格）来监视、搜索、分析和可视化度量值。您可以使用 Grafana 来执行高级分析任务。
{:shortdesc}

如果使用 Grafana，那么可以使用仪表板来创建使用度量值查询的图形。
1. [浏览至 Grafana 仪表板](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-navigating_grafana#navigating_grafana)。
2. 选择域 `account` 和具有链接到裸机设备的 IBM 标识的用户帐户。
3. 使用以下格式来创建查询。
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. 以下是可用的度量值类型：
<table>
   <CAPTION>表 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>类型</th>
     <th>单位</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>字节</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>字节</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>字节</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>字节</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>字节/秒</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>字节/秒</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>个操作/秒</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>个操作/秒</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>每个操作的等待时间，以毫秒为单位</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>每个操作的等待时间，以毫秒为单位</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` 或 net-private-in-bps-<id> net-private-in-bps-agg</td>
       <td>字节/秒</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` 或 net-private-out-bps-<id> net-private-out-bps-agg</td>
       <td>字节/秒</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` 或 `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>数字</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` 或 `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>数字</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` 或 `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>数字</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` 或 `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>数字</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>此度量值并非适用于所有设备。</td>
       <td>摄氏度</td>
     </tr>
   </TBODY>
   </table>

有关更多信息，请参阅[在 Grafana 中配置度量值查询](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-define_query#define_query)。
