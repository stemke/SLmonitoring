---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-27"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# Getting started with IBM Cloud Monitoring (Beta)

{: #gettingstartedbeta}

Built on the IBM Cloud Monitoring Service, this beta monitoring application for virtual servers is native to the IBM Cloud infrastructure, agentless, and is available on both current and future architectures.

{:shortdesc}

## Prerequisites

To participate in this Beta program, you must meet these requirements.
1. Your SoftLayer account must be linked to an IBM BlueMix account. To link an account, the Master User on your SoftLayer account must login to the {{site.data.keyword.slportal_full}}, and click **Link a Bluemix Account!**.
2. Each user to view the Beta must be linked to an IBM ID. For more information, see [Linking IBMid user accounts](../../cloud-platform/accounts/softlayerlink.html#link_user_accounts)
3. Each user to view the Beta must have an IAM policy that allows access to the monitoring service. 
   1. From the BlueMix Console,  select **Manage -> Account -> Users**.
   2. Invite the user to the account or select the user from the list.
   3. Select **Assign Policy** to the user.
   4. From **Service**, select **IBM Cloud Monitoring Service**. 
   5. Select the **Role** to be granted to the user.

If you do not meet these requisites, you are not able to access the Beta monitoring at this time.


## Joining the beta

Follow these steps to get started with the monitoring Beta program.

1. From a qualified account, click the **Device Name** to access the device details.
2. On the **Usage** tab, click the **Join** link to switch to the Beta view.
3. Review the currently available Beta monitoring data for this server.

|              Metrics                                      |  Description                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU Utilization                                            |   View the % of CPU utilization for up to 4 cores and total utilization. Click each    metric in the key to turn the data on or off on the graph.
|Public Network                                             |   View inbound and outbound data for your public network. Click each metic in the key to turn the data on or off on the graph.       |
|Private Network                                            |   View inbound and outbound data for your private network. Click each metic in the key to turn the data on or off on the graph.           |
|Memory utilization     | View the % of memory utilization for your server     |
{: caption="Table 1. Beta metrics" caption-side="top"}   


## Troubleshooting
To view some metrics, like memory utilization, xen tools are required on your server. For information on installing xen tools, see [Preparing and importing images](../image-templates/import-image.html#preparing-and-importing-images)

## Next Steps
To provide feedback on this Beta, use the link at the bottom on the **Usage** tab to complete a short survey. To leave the Beta and return to the standard view, click the ** Leave the Beta** link at the bottom of the **Usage** tab.


