---

copyright:
  years: 2014, 2020
lastupdated: "2020-05-13"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft, Sysdig, monitoring

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

# Getting started tutorial
{: #monitoring}

{{site.data.keyword.cloud}} is transitioning to I{{site.data.keyword.mon_full_notm}}. Nimsoft Monitor is available for purchase until the transition occurs. For more information about {{site.data.keyword.mon_full_notm}}, see [{{site.data.keyword.mon_full_notm}}](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-about). <!--For existing Nimsoft customers, Nimsoft support continues until the transition is complete. To continue monitoring after this date, you need to move to Sysdig.-->
{: important}

{{site.data.keyword.cloud}} offers {{site.data.keyword.mon_full_notm}} to keep you aware of any issues with your devices. {{site.data.keyword.mon_full_notm}} gives you insight into the performance and health of your applications, services, and platforms. Your administrators, DevOps teams, and developers have full stack telemetry with advanced features to help them monitor and troubleshoot, define alerts, and design custom dashboards.
{:shortdesc}

## Initiate service and slow pings

You use IBM Cloud Monitoring to initiate service and slow pings to make sure that the device is online and responsive.

If an echo isn't received in the allotted time frame (1 second for service pings, 5 seconds for slow pings), an alert is sent to the email address on the account. A status of **Up** in the **Status** field indicates that an echo was received, while **Down** indicates that the echo wasn't received.

To view configured monitors, follow these steps:

1. Go to your console's device menu. For more information, see [Navigating to devices](/docs/vsi?topic=virtual-servers-navigating-devices).
2. From the **Devices** menu, select **Device List** and select the device.
3. Click the **Monitoring** tab. All current pings are viewable on the landing page. 

## Getting started with Sysdig

For information about setting up an {{site.data.keyword.mon_full_notm}} monitoring agent, see [Getting started with {{site.data.keyword.mon_full_notm}}](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-getting-started).

The **Monitoring** tab is only visible if at least one monitor is configured.
{:note}

