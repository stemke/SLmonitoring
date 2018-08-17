---
copyright:
  years: 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 管理 IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent 会从其安装所在的设备收集度量值数据，并将这些数据发送到度量值存储器。度量值存储器中的数据可用于用户界面以进行简单监视，还可用于 Grafana 以进行高级查询。如果在您的服务器上使用 IBM Cloud Monitoring Service for IaaS Bare Metal Agent，请执行以下步骤来查看、停止、启动或卸载该服务。
{:shortdesc}

<table>
   <CAPTION>表 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>如果要执行的操作是...</th>
   <th>对于 Linux，请执行以下操作...</th>
     <th>对于 FreeBSD，请执行以下操作...</th>
     <th>对于 Windows，请执行以下操作...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>查看服务的状态</td>
   <td>
   使用命令 `service monitoring status`
   </td>
     <td>
   使用命令 `service monitoring status`
   </td>
     <td>
   使用命令 `sc.exe query monitoring`
   </td>
   </tr>
   <tr>
   <td>停止监视服务</td>
   <td>
   使用命令 `service monitoring stop`
   </td>
     <td>
   使用命令 `service monitoring stop`
   </td>
     <td>
   使用命令 `sc.exe stop monitoring`
   </td>
   </tr>
       <tr>
   <td>启动监视服务</td>
   <td>
   使用命令 `service monitoring start`
   </td>
     <td>
   使用命令 `service monitoring start`
   </td>
     <td>
   使用命令 `sc.exe start monitoring`
   </td>
   </tr>
       <tr>
   <td>卸载监视服务</td>
   <td>输入以下命令：<ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>输入以下命令：<ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>执行以下步骤：<ol>
       <li>打开**添加或删除程序**。</li>
       <li>选择 **IBM Cloud Monitoring Agent**</li>
   <li>单击**卸载**。</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>



