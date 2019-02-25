---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creating and managing system policies (Beta)
You can create policies to trigger notifications when your device reaches a predetermined monitoring threshold. For example, you can notify users if the average CPU usage of your device reaches a warning or error level. Only 10 monitoring policies can exist at one time. However, a policy can be applied to multiple devices.
{:shortdesc}


Follow these steps to work with your system policies.
1. After joining the beta, select **Devices -> Monitoring**.
2. Click the **System Policies** tab.

<table>
   <CAPTION>Table 1.Create and manage system policies</CAPTION>
   <THEAD>
   <TR>
   <th>If the action to be taken is...</th>
   <th>Then...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Create a policy</td>
   <td>
   <ol>
     <li>Click <b>Create Notification</b>.</li>
     <li>Enter the information for your new system policy.

<table>
  <caption>System policy details</caption>
  <tr>
     <th>Field</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Enter a unique identifier for your new system policy. This is a required field.</td>
  </tr>
  <tr>
    <td>Trigger</td>
    <td>Select the details that trigger your system policy. This can be different metric levels for warnings and errors. For example, <i>Average</i>.</td>
  </tr>
   <tr>
    <td>Duration</td>
     <td>Select how long an event occurs to trigger your policy.</td>
  </tr>
   <tr>
    <td>Device</td>
    <td>The device monitored for the policy.</td>
  </tr>
   <tr>
    <td>Default Notification</td>
    <td>Define the default notification for your policy.</td>
  </tr>
</table>
</li>
<li>Click <b>OK</b> to accept your changes.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Edit a policy</td>
   <td>
   <ol>
     <li>Click <b>Edit a Policy</b>.</li>
    <li>Enter the changed information for your system policy.

<table>
  <caption>System policy details</caption>
  <tr>
     <th>Field</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Enter a unique identifier for your new system policy. This is a required field</td>
  </tr>
  <tr>
    <td>Trigger</td>
    <td>Select the details that trigger your system policy. This can be different metric levels for warnings and errors.</td>
  </tr>
   <tr>
    <td>Duration</td>
     <td>Select how long an event occurs to trigger your policy.</td>
  </tr>
</table>
</li>
<li>Click <b>Ok</b> to accept your changes.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Remove a policy</td>
   <td>
   <ol>
     <li>Click <b>Actions->Delete policy</b>.</li>
     <li>Click <b>Delete</b> to confirm your choice.</li>
   </ol>
   </td>
   </tr>
   <tr>
  <td>Assign devices</td>
  <td>
    <ol>
      <li>Click <b>Manage devices</b>.</li>
      <li>Select or unselect devices to assign the policy.</li>
       <li>Click <b>OK</b> to accept your changes.</li>
    </ol>
      </td>
  </tr>
   <tr>
  <td>Duplicate a policy</td>
  <td>
    <ol>
      <li>Click <b>Actions->Duplicate policy</b>.</li>
      <li>Enter any changed information for your new policy.</li>
       <li>Click <b>OK</b> to accept your changes.</li>
    </ol>
      </td>
  </tr>

   </TBODY>
   </table>
