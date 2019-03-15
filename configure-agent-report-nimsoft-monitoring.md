---

copyright:
  years: 2014, 2017
lastupdated: "2017-10-30"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configuring a Nimsoft Monitoring agent report
{: #configuring-a-nimsoft-monitoring-agent-report}

1. From the monitoring screen, select **Configure Agent Reports** from the **Actions** drop-down menu in the **Advanced** column.

2. Select the agent to configure from the **Agents** drop-down list.
  * **Note:** Available agents vary by device and are dependent on the monitoring package applied to the device.

3. Select the section to configure from the **Sections** drop-down list. If you select a section that contains profiles, another drop-down list appears. From that list, select an **existing Profile** from the **Profiles** drop-down list. To add a new configuration, select **Add Agent Config...** from the **Profiles** drop-down list.

4. Complete each field in the **General metrics and information** section, if necessary.
  * **Note:** Required fields are indicated by a red asterisk (*). Not all agents, sections, or profiles contain this section.

5. Click the **Metric** check box for each metric to be included in the report from the **Select metrics to report on** section, if applicable.

6. Click the **Alarm** check box for each alarm to activate for the Agent from **Metric Alarms**.
  * **Note:** Not all alarms in this section are tied to a specific metric. Alarms are sent to each email address associated with the **Alarm Subscribers** section for the Agent.

7. Click **Save** to save the configuration. Click **Cancel** to cancel the action.
  * **Note:** The save button is disabled until you make a change to the current configuration.

## Next steps

After you successfully save the configuration, a confirmation message appears. If the configuration was unsuccessful, an error message appears with details about the error that occurred and how to fix the error. You can reconfigure agents at any time by repeating these steps.
