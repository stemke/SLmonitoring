---

copyright:
  years: 2017
lastupdated: "2017-09-28"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Viewing and managing monitors

Monitoring a device allows users to initiate service and slow pings to ensure that the device is online and responsive.
{:shortdesc}

If an echo is not received in the allotted time frame (1 second for service pings, 5 seconds for slow pings) an alert is sent to the email
address on the account. A status of **Up** in the **Status** field indicates that an echo was received, while **Down**
indicates that the echo was not received. If you have a configured basic monitor, follow these steps to view and manage monitoring for a device.

   <table>
   <CAPTION>Table 1. View and manage device monitoring</CAPTION>
   <THEAD>
   <TR>
   <th>If the action to be taken is...</th>
   <th>Then...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>View monitors</td>
   <td>
   <ol>
   <li>From the Device List, click the <b>Device Name</b> to access the device.</li>
   <li>Click the <b>Monitoring</b> tab. All current pings are viewable on the landing page. (The <b>Monitoring</b> tab is only visible if at least one monitor is configured.)</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Add a monitor</td>
   <td>
   <ol>
   <li>From the <b>Monitoring</b> tab of the Device Details page, click <b>Manage Monitors</b> on the right side of the page to manage monitors associated with this device.</li>
   <li>On the Monitors page, click the <b>Add Monitor</b> tab.</li>
   <li>Select the IP address to monitor from the <b>IP Address</b> list.</li>
   <li>Select the monitor type from the <b>Monitor Type</b> list.</li>
   <li>Set up the notification options. From the <b>Notify?</b> list, select <b>Notify Users</b> to notify users of issues, or <b>Do Nothing</b> to bypass user notification.</li>
   <li>Select the time frame for user notification from the use <b>Notify Wait</b> list.</li>
   <li>Click <b>Add Monitor</b> to add the monitor for the device. The new monitor appears in the <b>Edit Existing Monitors</b> section of the screen.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Edit an existing monitor</td>
   <td>
   <ol>
   <li>On the Monitors page under the <b>Edit Existing Monitors</b> heading, click any of the monitor details to open the monitor for edits.</li>
   <li>Update any of the following fields: Monitor Type, Notify, Notify Wait.</li>
   <li>Click <b>Update</b> to update the details. Click <b>Cancel</b> to cancel the edit.</li>
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
- If a monitor is edited, the monitor continues to function as specified in the monitor details. If type is changed, the amount of time to receive the expected ping is different. If notification options changed, the way users are notified of a failed attempt is changed based on the new selections. The monitor remains accessible from the **Monitoring** tab.
- If a monitor is removed, the monitor no longer functions for the device. All monitoring that is associated with the removed monitor stops, and the monitor no longer appears on the **Monitoring** tab.
