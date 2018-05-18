---
copyright:
  years: 1994, 2017
lastupdated: "2017-06-09"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Adding and removing monitors

<table>
   <CAPTION>Table 1. Adding and removing device monitors</CAPTION>
   <THEAD>
   <TR>
   <th>If the action to be taken is...</th>
   <th>Then...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Add a monitor</td>
   <td>
   <ol>
   <li>From the <b>Monitoring</b> tab of the Device Details page, click <b>Manage Monitors</b> on the right side of the page to manage monitors that are associated with this device.</li>
   <li>On the Monitors page, click the <b>Add Monitor</b> tab.
   * **Note:** Public and Private IP addresses are available for monitoring. Each IP address is identified on the **Server Info** tab.</li>
   <li>Select the IP address to monitor from the <b>IP Address</b> drop down list.</li>
   <li>Select the monitor type from the <b>Monitor Type</b> drop down list.</li>
   <li>Set up the notification options. From the <b>Notify?</b> drop down list, select <b>Notify Users</b>  notify users of issues, or <b>Do Nothing</b> to bypass user notification.</li>
   <li>Select the time frame for user notification from the use <b>Notify Wait</b> drop down list.</li>
   <li>Click <b>Add Monitor</b> to add the monitor for the device. The new monitor appears in the <b>Edit Existing Monitors</b> section of the screen.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Remove a monitor</td>
   <td>
   <ol>
   <li>On the Monitors page under the <b>Edit Existing Monitors</b> heading, click the Remove icon next to the monitor details.</li>
   <li>Click <b>Yes</b> to remove the monitor. Click <b>No</b> to cancel the action.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
   </table>


## Next steps

- If a new monitor is added, the monitor appears on the **Monitoring** tab. The monitor sends a ping to the device every 5 minutes, expecting a response based on the selected ping type. If the expected response is not received, an email is sent to the notification email address for the account in the specified time frame, if notification is selected.

- If a monitor is removed, the monitor will no longer function for the device. All monitoring that is associated with the removed monitor ceases, and the monitor no longer appears on the Monitoring tab.
