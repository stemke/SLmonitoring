---

copyright:
  years: 2017, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:note: .note}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Viewing and managing monitors
{: #viewing-and-managing-monitors}

Monitoring a device allows you to initiate service and slow pings to ensure that the device is online and responsive.
{:shortdesc}

If an echo is not received in the allotted time frame (1 second for service pings, 5 seconds for slow pings) an alert is sent to the email address on the account. A status of **Up** in the **Status** field indicates that an echo was received, while **Down** indicates that the echo was not received. If you have a configured basic monitor, follow these steps to view and manage monitoring for a device.

## Before you begin
{: #before-you-begin-monitors}

First, navigate to the device menu and ensure you have the correct account permissions to complete the tasks.

* Navigate to your console's device menu. For more information, see [Navigating to devices](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Ensure you have any necessary account permissions and device access. Only the account owner, or a user with the **Manage Users** classic infrastructure permission, can adjust the permissions.

For more information about permissions, see [Classic infrastructure permissions](/docs/iam?topic=iam-infrapermission#infrapermission) and [Managing device access](/docs/vsi?topic=virtual-servers-managing-device-access).

## Viewing monitors
{: #viewing-monitors}

1. From the **Devices** menu, select **Device List**.
2. Click the device name to access the device.
3. Click the **Monitoring** tab. All current pings are viewable on the landing page.

The **Monitoring** tab is only visible if at least one monitor is configured.
{:note}

## Adding a monitor
{: #adding-a-monitor}

1. From the **Devices** menu, select **Device List**.
2. Click the device name to access the device.
3. Click the **Monitoring** tab, and select **Manage monitors**.
4. Select **Add Monitor**.
5. Select the IP address to monitor in the **IP Address** field and the monitor type in the **Monitor Type** field. 
6. Set up the notification options. In the **Notify ?** field, select **Notify Users** to notify users of issues, or select **Do Nothing** to bypass user notification.
7. Select the timeframe for user notification in the **Notify Wait** field.
8. Click **Add Monitor** to add the monitor to the device. The new monitor appears in the **Edit Existing Monitors** section.

## Editing an existing monitor
{: #editing-an-exisiting-monitor}

1. From the **Devices** menu, select **Device List**.
2. Click the device name to access the device.
3. Click the **Monitoring** tab, and select **Manage monitors**.
4. In the **Edit Existing Monitors** section, click any of the monitor details to open the monitor for edits.
5. Update any of the following fields: **Monitor Type, Notify,** or **Notify Wait**.
6. Click **Update** to update the details.

## Removing a monitor
{: #removing-a-monitor}

1. From the **Devices** menu, select **Device List**.
2. Click the device name to access the device.
3. Click the **Monitoring** tab, and select **Manage monitors**.
4. In the **Edit Existing Monitors** section, click the **Remove** icon in the monitor details.
5. Select **Yes** to remove the monitor.

## Next steps
{: #next-steps-managing-monitors}

- If a new monitor is added, the monitor appears on the **Monitoring** tab. The monitor sends a ping to the device every 5 minutes, expecting a response based on the selected ping type. If the expected response is not received, an email is sent to the notification email address for the account in the specified time frame, if notification is selected.
- If a monitor is edited, the monitor continues to function as specified in the monitor details. If type is changed, the amount of time to receive the expected ping is different. If notification options changed, the way users are notified of a failed attempt is changed based on the new selections. The monitor remains accessible from the **Monitoring** tab.
- If a monitor is removed, the monitor no longer functions for the device. All monitoring that is associated with the removed monitor stops, and the monitor no longer appears on the **Monitoring** tab.

