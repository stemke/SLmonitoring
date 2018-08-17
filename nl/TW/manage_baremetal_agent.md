---
copyright:
  years: 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 管理 IBM Cloud Monitoring Service for IaaS Bare Metal Agent（測試版）

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent 會從其安裝所在的裝置中收集度量資料，並將它傳送至度量儲存空間。從度量儲存空間中，資料可供使用者介面用於簡單監視，以及可供 Grafana 用於進階查詢。如果您是使用 IBM Cloud Monitoring Service for IaaS Bare Metal Agent，請遵循下列步驟來檢視、停止、啟動或解除安裝伺服器的服務。
{:shortdesc}

<table>
   <CAPTION>表 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>如果要採取的動作是...</th>
   <th>若是 Linux，則...</th>
     <th>若是 FreeBSD，則...</th>
     <th>若是 Windows，則...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>檢視服務的狀態</td>
   <td>
   使用指令 `service monitoring status`
   </td>
     <td>
   使用指令 `service monitoring status`
   </td>
     <td>
   使用指令 `sc.exe query monitoring`
   </td>
   </tr>
   <tr>
   <td>停止監視服務</td>
   <td>
   使用指令 `service monitoring stop`
   </td>
     <td>
   使用指令 `service monitoring stop`
   </td>
     <td>
   使用指令 `sc.exe stop monitoring`
   </td>
   </tr>
       <tr>
   <td>啟動監視服務</td>
   <td>
   使用指令 `service monitoring start`
   </td>
     <td>
   使用指令 `service monitoring start`
   </td>
     <td>
   使用指令 `sc.exe start monitoring`
   </td>
   </tr>
       <tr>
   <td>解除安裝監視服務</td>
   <td>請輸入下列指令：
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>請輸入下列指令：
     <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>請遵循下列步驟：
 <ol>
       <li>開啟**新增或移除程式**。</li>
       <li>選取 **IBM Cloud Monitoring Agent**。</li>
   <li>按一下**解除安裝**。</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>



