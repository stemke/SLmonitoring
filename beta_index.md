---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

keywords: IBM Cloud Monitoring Service

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Getting started with IBM Cloud Monitoring (Beta)
{: #getting-started-with-ibm-cloud-monitoring-beta}

This beta monitoring application, built on the {{site.data.keyword.BluSoftlayer_full}} Monitoring Service is available for virtual and bare metal servers. For updates on the development of this Beta program, see the [IBM Cloud Blog ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}.
{:shortdesc}

## Prerequisites

To participate in this Beta program, you must meet these requirements.
1. Your SoftLayer account must be linked to an IBM Cloud account with IBMid authentication. To link an account, the Master User on your SoftLayer account must log in to the [{{site.data.keyword.slportal}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com){: new_window}, and from the **Account** menu, click **Link a Bluemix Account!**.
2. Each user to view the Beta must be linked to an IBM ID. For more information, see [Linking IBMid user accounts](/docs/account?topic=account-unifyingaccounts#link_customer_accounts).
3. Each user to view the Beta must have access to the IBM Cloud Monitoring Service.
   1. From the [IBM Cloud console ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://console.bluemix.net){: new_window},  select **Manage -> Account -> Users**.
   2. Invite the user to the account or select the user from the list.
   3. Select **Assign Access to Resources** to the user.
   4. From **Service**, select **IBM Cloud Monitoring Service**.
   5. Select the **Role** to be granted to the user for all regions.

If you do not meet these prerequisites, you are not able to access the Beta monitoring at this time.


## Joining the beta

Follow these steps to get started with the monitoring Beta program. Joining the Beta enables the service for all eligible virtual and bare metal servers in your account. Clicking join does not affect existing Nimsoft monitoring or data.
1. (Bare metal only) [Install the monitoring agent on your bare metal server](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-).
<table>
   <CAPTION>Table 1. Choose a log in location</CAPTION>
   <THEAD>
   <TR>
   <th>If you want to join with the...</th>
   <th>Then...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>IBM Cloud catalog</td>
   <td>
   <ol>
   <li>Open a new browser window and enter  <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>.</li>
   <li>Click the <b>Log in</b> link. </li>
   <li>Enter your email or IBMid and click <b>Continue.</b></li>
   <li>Enter your Password and click <b>Log in.</b></li>
   <li>Select **Infrastructure->Device List->*Device Name*** to access the device details.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Customer Portal</td>
   <td>
   <ol>
   <li>Open a new browser window and enter <a href="https://control.softlayer.com">https://control.softlayer.com</a>.</li>
   <li>Type your user name and Password, and click <b>Log In</b>. Or, click <b>Log in with IBMid</b>. Then, enter your email or IBMid and click <b>Continue</b>. Enter your password and click <b>Log In</b>. The main page of the {{site.data.keyword.slportal}} opens.</li>
     <li>From **Devices**, click the **Device Name** to access the device details.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. Select **Devices -> Monitoring**. Click **Join the beta** to view the system policies and notifications beta tabs.

## Next steps
1. Review the details of collected [metrics](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-).
2. [Create or manage](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-) a monitor notification.
3. [Create or manage](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-) a system policy.
4. [View alerts](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-).
5. Review the currently available Beta monitoring graph data for a selected device.

|              Metrics                                      |  Description                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU utilization                                            |   View the % CPU utilization for each core and an average across cores. Click each    metric in the key to turn the data on or off on the graph.
|Public network                                             |   View inbound and outbound data for your public network. Click each metric in the key to turn the data on or off on the graph.       |
|Private network                                            |   View inbound and outbound data for your private network. Click each metric in the key to turn the data on or off on the graph.           |
|Memory utilization    | View the % of memory utilization for your server     |
|Disk usage    | View the average amount of data being read or written from or to disk in bytes or the disk latency. Click each metric in the key to turn the data on or off on the graph.    |
|Temperature                                                 |View the temperature of your bare metal device in degrees Celsius. This data is not available for all devices.
{: caption="Table 2. Beta metrics" caption-side="top"}   

## Limitations
If a device is deleted, associated monitoring policies are not deleted. Be aware that you must manually delete the device for these policies.

Metrics data is available for 15 days only.

Only 10 monitoring policies can exist at one time. However, a policy can be applied to multiple devices.

## Troubleshooting
To view some metrics, like memory utilization, Xen tools are required on your server. For information on installing Xen tools, see [Preparing and importing images](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images).

## Feedback
To provide feedback on this Beta, select **Devices -> Monitoring** or the device details page and click **Leave feedback** to complete a short survey. To leave the Beta and return to the standard view, click the **Leave the Beta** link at the bottom of the **Devices -> Monitoring** page.
