---
copyright:
  years: 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creating and managing monitor notifications (Beta)
A notification describes the method and details that is used to notify when an alert is triggered. For example, to get a warning notification and an error notification for a metric, define a rule that monitors the warning threshold, and define a rule that monitors the error threshold.
{:shortdesc} 

## Create a notification
 
 1. After you have joined the beta, select **Devices -> Monitoring**. 
 2. Click the **Notifications** tab.
 3. Click **Create Notification**.
 4. Enter the information for your new notification. 

<table>
  <caption>Email notification details</caption>
  <tr>
     <th>Field</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>A unique identifier of the notification. This field is required.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Select: **Email**</td>
  </tr>
  <tr>
    <td>Email Address</td>
    <td>Enter the email address of the recipient.</td>
  </tr>
</table>

<table>
  <caption>Webhook notification details</caption>
  <tr>
     <th>Field</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>A unique identifier of the notification. This field is required.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Select: **Webhook**</td>
  </tr>
  <tr>
    <td>Webhook URL</td>
    <td>Enter the URL where the POST should be made.</td>
  </tr>
  <tr>
  <td>Verify certificates</td>
    <td>Select to verify certificates.</td>
  </tr>
  <tr>
    <td>Webhook headers</td>
    <td>Enter any headers.</td>
  </tr>
  <tr>
    <td>Webhook query parameters</td>
    <td>Enter any query parameters.</td>
  </tr>
</table>

<table>
  <caption>Pager duty notification details</caption>
  <tr>
     <th>Field</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>A unique identifier of the notification. This field is required.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Select: **Pager duty**</td>
  </tr>
  <tr>
    <td>API Key</td>
    <td>Enter the enter the APIKey for pager duty notifications.</td>
  </tr>
</table>


5. Click **Ok** to create the new notifications with the setting you speficied.

## Edit a notification
 1. After you have joined the beta, select **Devices -> Monitoring**. 
 2. Click the **Notifications** tab.
3. Click **Actions->Edit Notification**.
4. Edit any of the notification details.
5. Click **Ok** to accept your changes.

## Delete a notification
1. After you have joined the beta, select **Devices -> Monitoring**. 
2. Click the **Notifications** tab.
3. Click **Actions->Delete Notification**.
4. Click **Delete** to confirm your choice.

## Add multiple notifications to a device
1. Select **Infrastructure->Device List->*Device Name*** to access the device details.
2. Click **Actions->Manage notifications**.
4. Click to assign or remove notifications for your device.

