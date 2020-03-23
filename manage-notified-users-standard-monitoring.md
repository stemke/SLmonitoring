---

copyright:
  years: 2014, 2019
lastupdated: "2019-08-23"

keywords: monitoring, notified users

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Managing notified users for standard monitoring
{: #managing-notified-users-for-standard-monitoring}

Notified users for the standard monitoring service receive automated notifications anytime a device does not respond to a ping in the allotted response time. You can add or remove notified users anytime, and notified users must be on the account associated with the device to receive a notification. Follow these steps to manage notified users for the standard monitoring service.
{:shortdesc}

## Before you begin
{: #byb-notified-users}

First, navigate to the device menu and ensure you have the correct account permissions to complete the tasks.

* Navigate to your console's device menu. For more information, see [Navigating to devices](/docs/SLmonitoring?topic=virtual-servers-navigating-devices).
* Ensure you have any necessary account permissions and device access. Only the account owner, or a user with the **Manage Users** classic infrastructure permission, can adjust the permissions.

For more information about permissions, see [Classic infrastructure permissions](/docs/iam?topic=iam-infrapermission#infrapermission) and [Managing device access](/docs/vsi?topic=virtual-servers-managing-device-access).

## Adding notified users
{: #adding-notified-users}

Complete the following steps to add notified users for the standard monitoring service.
1. From the **Device** menu, select **Device List**.
2. Click the device name to access the device.
3. Click the **Monitoring** tab, and select **Manage monitors**.
4. Select **Manage Notified Users**.
5. From the **Users to Notify** drop-down list, select the new user to notify.
6. Select **Add User**.

## Removing notified users
{: #removing-notified-users}

Complete the following steps to remove notified users for the standard monitoring service.
1. From the **Device** menu, select **Device List**.
2. Click the device name to access the device.
3. Click the **Monitoring** tab, and select **Manage monitors**.
4. Select **Manage Notified Users**.
5. Click the **Remove** icon to remove the existing notified user, then select **Yes** to remove the user. 

## Next steps
{: #ns-notified-users}

If you add a notified user, the user is notified of any missed ping responses. If you removed a notified user, the user no longer receives a notification of missed ping responses associated with the device.
