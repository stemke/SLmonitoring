---

copyright:
  years: 2014, 2018
lastupdated: "2018-10-30"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Editing an existing monitor
After a monitor is added to a device, you can modify or remove it at any time. Modifications to monitors allow for changes to the type and notification options, while removing a monitor cancels the monitor completely. Follow these steps to edit an existing monitor.

1. On the **Monitors** page under the **Edit Existing Monitors** heading, click any of the monitor details to open the monitor for editing.

2. Modify the **Monitor Details** as necessary. Refer to this table for more details on each editable field.

|Field|Details|Action|
|---|---|---|
|Monitor Type|The amount of time in which a response from the device is expected. The system defaults to a service ping. A slow ping waits 5 seconds for a reply, allowing servers that are optimized for non-network tasks more time to process the request. A service ping issues one ping every 5 minutes and expects an echo reply within 1 second. If more than one ping is missed, an alert is issued.|Select from **Slow Ping** or **Service Ping**.|
|Notify| Notified users receive automated notifications any time a device does not respond to a ping in the allotted response time. For notification, a user must be on the account associated with the device to receive a notification.|To add a user, select the new **Notified User**, and click **Add User**. To remove a user, click the **Remove** icon next to the existing Notified User and click **Yes** to confirm your action.|
|Notify Wait|The amount of time the system waits to send a notification when the device did not respond to the ping. Multiple wait times are available. **Note:** Notify details are not required when no users are selected for notification. |Select the wait time you need.|

3. Click **Update** to apply the changes to the monitor. Click  **Cancel** to cancel the action.

## Next steps

If a monitor is edited, the monitor continues to function as specified in the monitor details. If type is changed, the amount of time to receive the expected ping is different. If notification options change, the notification mode is changed based on the new selections. The monitor remains accessible from the monitoring tab.
