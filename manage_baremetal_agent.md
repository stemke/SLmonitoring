---

copyright:
  years: 2018
lastupdated: "2018-03-29"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Managing the IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)
{: #managing-the-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta}

The {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent collects metric data from the device on which it's installed and sends it to metric storage. From metric storage, the data is available to the user interface for simple monitoring and Grafana for advanced queries.
If you are using the IBM Cloud Monitoring Service for IaaS Bare Metal Agent, follow these steps to view, stop, start, or uninstall the service for your server.
{:shortdesc}

<table>
   <CAPTION>Table 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>If the action to be taken is...</th>
   <th>Then, for Linux...</th>
     <th>Then, for FreeBSD...</th>
     <th>Then, for Windows...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>View the status of the service</td>
   <td>
   Use the command `service monitoring status`
   </td>
     <td>
   Use the command `service monitoring status`
   </td>
     <td>
   Use the command `sc.exe query monitoring`
   </td>
   </tr>
   <tr>
   <td>Stop the monitoring service</td>
   <td>
   Use the command `service monitoring stop`
   </td>
     <td>
   Use the command `service monitoring stop`
   </td>
     <td>
   Use the command `sc.exe stop monitoring`
   </td>
   </tr>
       <tr>
   <td>Start the monitoring service</td>
   <td>
   Use the command `service monitoring start`
   </td>
     <td>
   Use the command `service monitoring start`
   </td>
     <td>
   Use the command `sc.exe start monitoring`
   </td>
   </tr>
       <tr>
   <td>Uninstall the monitoring service</td>
   <td>Enter these commands:
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>Enter these commands:
  <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>Follow these steps:
 <ol>
       <li>Open **Add or Remove Programs**.</li>
       <li>Select **IBM Cloud Monitoring Agent**</li>
   <li>Click **Uninstall**.</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>
