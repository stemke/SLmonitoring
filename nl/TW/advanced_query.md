---
copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 建立進階監視查詢（測試版）

在 {{site.data.keyword.cloud}} 中，您可以使用 Grafana（一種開放程式碼分析與視覺化平台），以各種圖形（例如圖表和表格）監視、搜尋、分析及視覺化您的度量值。您可以使用 Grafana 來執行進階分析作業。
{:shortdesc}

如果您使用 Grafana，則可以使用儀表板來利用度量查詢建立圖形。
1. [導覽至 Grafana 儀表板](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/navigating_grafana.html#navigating_grafana)。
2. 以鏈結至裸機裝置的 IBM ID 來選取網域`帳戶`及使用者帳戶。 
3. 使用此格式來建立查詢。
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. 以下是可用的度量類型：
<table>
   <CAPTION>表 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>類型</th>
     <th>單位</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>百分比</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>位元組數</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>百分比</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>位元組數</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>百分比</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>位元組數</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>位元組數</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>百分比</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>位元組數/秒</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>位元組數/秒</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>作業數/秒</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>作業數/秒</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>以毫秒表示每個作業的延遲</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>以毫秒表示每個作業的延遲</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` 或 `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>位元組數/秒</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` 或 `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>位元組數/秒</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` 或 `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>數字</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` 或 `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>數字</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` 或 `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>數字</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` 或 `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>數字</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>此度量不適用於所有裝置。</td>
       <td>度（攝氏）</td>
     </tr>
   </TBODY>
   </table>

如需相關資訊，請參閱[在 Grafana 中配置度量值查詢](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/define_query.html#define_query)。
