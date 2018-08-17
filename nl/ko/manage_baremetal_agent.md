---
copyright:
  years: 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# IBM Cloud Monitoring Service for IaaS Bare Metal Agent 관리(베타)

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent는 이 에이전트가 설치된 디바이스에서 지표 데이터를 수집하여 지표 스토리지에 전송합니다. 지표 스토리지의 데이터는 사용자 인터페이스에서 단순 모니터링을 위해 사용하고 Grafana에서 고급 조회를 위해 사용할 수 있습니다.
IBM Cloud Monitoring Service for IaaS Bare Metal Agent를 사용 중인 경우 서버에 대한 서비스를 확인, 중지, 시작 또는 설치 제거하려면 다음 단계를 따르십시오.
{:shortdesc}

<table>
   <CAPTION>표 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>수행해야 하는 조치</th>
   <th>Linux의 경우 수행할 작업</th>
     <th>FreeBSD의 경우 수행할 작업</th>
     <th>Windows의 경우 수행할 작업</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>서비스의 상태 보기</td>
   <td>
   `service monitoring status` 명령 사용
   </td>
     <td>
   `service monitoring status` 명령 사용
   </td>
     <td>
   `sc.exe query monitoring` 명령 사용
   </td>
   </tr>
   <tr>
   <td>모니터링 서비스 중지</td>
   <td>
   `service monitoring stop` 명령 사용
   </td>
     <td>
   `service monitoring stop` 명령 사용
   </td>
     <td>
   `sc.exe stop monitoring` 명령 사용
   </td>
   </tr>
       <tr>
   <td>모니터링 서비스 시작</td>
   <td>
   `service monitoring start` 명령 사용
   </td>
     <td>
   `service monitoring start` 명령 사용
   </td>
     <td>
   `sc.exe start monitoring` 명령 사용
   </td>
   </tr>
       <tr>
   <td>모니터링 서비스 설치 제거</td>
   <td>다음 명령을 입력하십시오.
<ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>다음 명령을 입력하십시오.
<ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>다음 단계를 수행하십시오.
 <ol>
       <li>**프로그램 추가 또는 제거**를 여십시오.</li>
       <li>**IBM Cloud Monitoring Agent**를 선택하십시오.</li>
   <li>**설치 제거**를 클릭하십시오.</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>



