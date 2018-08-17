---
copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 고급 모니터링 조회 작성(베타)

{{site.data.keyword.cloud}}에서 오픈 소스 분석 및 시각화 플랫폼인 Grafana를 사용하여 차트 및 표와 같은 다양한 그래프로 지표를 모니터, 검색, 분석 및 시각화할 수 있습니다. Grafana를 사용하여 고급 분석 태스크를 수행할 수 있습니다.
{:shortdesc}

Grafana를 사용하는 경우 대시보드를 사용하여 지표 조회를 사용하는 그래프를 작성할 수 있습니다.
1. [Grafana 대시보드로 이동](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/navigating_grafana.html#navigating_grafana)하십시오.
2. `account` 도메인 및 베어메탈 디바이스에 연결된 IBM ID가 있는 사용자 계정을 선택하십시오. 
3. 다음 형식을 사용하여 조회를 작성하십시오.
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. 다음은 사용 가능한 지표 유형입니다.
<table>
   <CAPTION>표 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>유형</th>
     <th>단위</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>바이트</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>바이트</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>바이트</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>바이트</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>바이트/초</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>바이트/초</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>오퍼레이션/초</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>오퍼레이션/초</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>오퍼레이션당 대기 시간(밀리초)</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>오퍼레이션당 대기 시간(밀리초)</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` 또는 `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>바이트/초</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` 또는 `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>바이트/초</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` 또는 `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>수</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` 또는 `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>수</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` 또는 `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>수</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` 또는 `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>수</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>이 지표는 일부 디바이스에서만 사용 가능합니다.</td>
       <td>섭씨 온도</td>
     </tr>
   </TBODY>
   </table>

자세한 정보는 [Grafana에서 지표 조회 구성](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/define_query.html#define_query)을 참조하십시오.
