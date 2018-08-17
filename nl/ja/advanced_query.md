---
copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 拡張モニタリング照会の作成 (ベータ)

{{site.data.keyword.cloud}} では、分析および視覚化のためのオープン・ソース・プラットフォームである Grafana を使用して、さまざまなグラフ (図表や表など) でメトリックのモニター、検索、分析、および視覚化を行うことができます。Grafana を使用して、高度な分析タスクを実行できます。
{:shortdesc}

Grafana を使用する場合は、ダッシュボードでメトリック照会を使用してグラフを作成できます。
1. [Grafana ダッシュボードにナビゲートします](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/navigating_grafana.html#navigating_grafana)。
2. ドメインの`アカウント`と、ベア・メタル・デバイスにリンクされた IBM ID を持つユーザー・アカウントを選択します。 
3. 次の形式を使用して、照会を作成します。
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. 使用可能なメトリック・タイプは以下のとおりです。
<table>
   <CAPTION>表 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>タイプ</th>
     <th>単位</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>バイト</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>バイト</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>バイト</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>バイト</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>バイト数/秒</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>バイト数/秒</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>操作数/秒</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>操作数/秒</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>操作ごとの待ち時間 (ミリ秒)</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>操作ごとの待ち時間 (ミリ秒)</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` または `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>バイト数/秒</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` または `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>バイト数/秒</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` または `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>数</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` または `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>数</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` または `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>数</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` または `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>数</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>このメトリックは、すべてのデバイスで使用できるわけではありません。</td>
       <td>度 (摂氏)</td>
     </tr>
   </TBODY>
   </table>

詳しくは、[Grafana でのメトリック照会の構成](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/define_query.html#define_query)を参照してください。
