---

copyright:
  years: 2014, 2020
lastupdated: "2020-02-20"

keywords: monitoring, Nimsoft Monitoring, agent report

subcollection: SLmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:external: target="_blank" .external}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:important: .important}
{:note: .note}
{:tip: .tip}
{:deprecated: .deprecated}

# Viewing an agent report for Nimsoft Monitoring
{: #viewing-an-agent-report-for-nimsoft-monitoring}

Nimsoft Monitor is no longer available for purchase as {{site.data.keyword.cloud}} transitions to IBM Cloud Monitoring with Sysdig. For more information about Monitoring with Sysdig, see [IBM Cloud Monitoring with Sysdig](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-about). For existing Nimsoft customers, Nimsoft support continues until the transition is complete. To continue monitoring after this date, you need to move to Sysdig. 
{: important}

Monitoring details for Nimsoft Monitoring are available in agent reports, which provide the details specific to the way the agent was configured. 
{:shortdesc}

## Before you begin
{: #byb-viewing-an-agent-report-for-nimsoft-monitoring}

First, navigate to the device menu and ensure you have the correct account permissions to complete the tasks.

* Navigate to your console's device menu. For more information, see [Navigating to devices](/docs/SLmonitoring?topic=virtual-servers-navigating-devices).
* Ensure you have any necessary account permissions and device access. Only the account owner, or a user with the **Manage Users** classic infrastructure permission, can adjust the permissions.

For more information about permissions, see [Classic infrastructure permissions](/docs/iam?topic=iam-infrapermission#infrapermission) and [Managing device access](/docs/vsi?topic=virtual-servers-managing-device-access).

## Viewing an agent report for Nimsoft Monitoring
{: #viewing-agent-report-nimsoft-monitoring-steps}

Complete the following steps to view an agent report for Nimsoft Monitoring.

1. From the **Monitoring** page, select **View Agent Reports** from the **Actions** menu.
2. Select the agent to view from the **Agents** list.

  Available agents vary by device and are dependent on the monitoring package applied to the device.
  {:note}
  
3. Complete all remaining sections, including one or more of the following actions:

  Each agent varies and doesn't include each section or metric. Available options on this screen are dependent on the configuration options available for each agent.
  {:note}
  
  * Select the section report from the **Sections** list.
  * Select the time period for the report from the **View By** list.
  * Click the check box for each metric you want to report in the **Select metrics to report on:** section.
    
    Only similar metrics appear on the same graph. If conflicting metrics are chosen, an error occurs after you request the graph.
    {:note}
4. Click **Draw Graph** to draw the graph.

## Next steps
{: #ns-viewing-an-agent-report-for-nimsoft-monitoring}

After drawing the graph for the agent report, the graph can be redrawn at any time to view different metrics by repeating these steps. There's no limit to the number of agent reports that can be generated within a set amount of time.
