---

copyright:
  years: 2014, 2019
lastupdated: "2019-08-23"

keywords: monitoring, Nimsoft, Nimsoft Monitoring agent report

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

# Configuring a Nimsoft Monitoring agent report
{: #configuring-a-nimsoft-monitoring-agent-report}

Nimsoft Monitor is no longer available for purchase as {{site.data.keyword.cloud}} transitions to IBM Cloud Monitoring with Sysdig. For more information about Monitoring with Sysdig, see [IBM Cloud Monitoring with Sysdig](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-about). For existing Nimsoft customers, Nimsoft support continues until the transition is complete. To continue monitoring after this date, you need to move to Sysdig. 
{: important}

## Before you begin
{: #byb-configuring-a-nimsoft-monitoring-agent-report}

First, navigate to the device menu and ensure you have the correct account permissions to complete the tasks.

* Navigate to your console's device menu. For more information, see [Navigating to devices](/docs/SLmonitoring?topic=virtual-servers-navigating-devices).
* Ensure you have any necessary account permissions and device access. Only the account owner, or a user with the **Manage Users** classic infrastructure permission, can adjust the permissions.

For more information about permissions, see [Classic infrastructure permissions](/docs/iam?topic=iam-infrapermission#infrapermission) and [Managing device access](/docs/vsi?topic=virtual-servers-managing-device-access).

## Configuring a Nimsoft Monitoring agent report
{: #configuring-nimsoft-monitoring-agent-report-steps}

Complete the following steps to configure a Nimsoft Monitoring agent report.

1. From the **Devices** menu, select **Monitoring**.
2. From the **Monitoring** page, select **Configure Agent Reports** from the **Actions** drop-down menu in the **Advanced** column.
3. Select the agent to configure from the **Agents** drop-down list.
  
  Available agents vary by device and are dependent on the monitoring package applied to the device.
  {:note}

4. Select the section to configure from the **Sections** drop-down list. If you select a section that contains profiles, another drop-down list appears. From that list, select an **existing Profile** from the **Profiles** drop-down list. To add a new configuration, select **Add Agent Config...** from the **Profiles** drop-down list.

5. Complete each field in the **General metrics and information** section, if necessary.
  
  Required fields are indicated by a red asterisk (*). Not all agents, sections, or profiles contain this section.
  {:note}

6. Click the **Metric** check box for each metric to be included in the report from the **Select metrics to report on** section, if applicable.

7. Click the **Alarm** check box for each alarm to activate for the Agent from **Metric Alarms**.

  Not all alarms in this section are tied to a specific metric. Alarms are sent to each email address associated with the **Alarm Subscribers** section for the Agent.
  {:note}

7. Click **Save** to save the configuration. Click **Cancel** to cancel the action.
  
  The **Save** button is disabled until you make a change to the current configuration.
  {:note}

## Next steps
{: #ns-configuring-a-nimsoft-monitoring-agent-report}

After you successfully save the configuration, a confirmation message appears. If the configuration was unsuccessful, an error message appears with details about the error that occurred and how to fix the error. You can reconfigure agents at any time by repeating these steps.
