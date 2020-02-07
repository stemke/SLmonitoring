---

copyright:
  years: 2014, 2020
lastupdated: "2020-02-07"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft, Sysdig, monitoring

subcollection: slmonitoring

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

As of 31 January 2020 Nimsoft Monitor is no longer available for purchase as {{site.data.keyword.cloud}} transitions to IBM Cloud Monitoring with Sysdig. For more information about Monitoring with Sysdig, see [IBM Cloud Monitoring with Sysdig](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-about). For existing Nimsoft customers, Nimsoft support continues until 31 May 2020. To continue monitoring after this date, you need to move to Sysdig. 
{: deprecated}

{{site.data.keyword.cloud}} offers Sysdig monitoring to keep you aware of any issues with your devices. Sysdig gives you insight into the performance and health of your applications, services, and platforms. Your administrators, DevOps teams, and developers have full stack telemetry with advanced features to help them monitor and troubleshoot, define alerts, and design custom dashboards.
{:shortdesc}

Windows Sysdig support is coming soon!
{:note}

## Initiate service and slow pings

You use IBM Cloud Monitoring to initiate service and slow pings to make sure that the device is online and responsive.

If an echo isn't received in the allotted time frame (1 second for service pings, 5 seconds for slow pings), an alert is sent to the email address on the account. A status of **Up** in the **Status** field indicates that an echo was received, while **Down** indicates that the echo wasn't received.

To view configured monitors, follow these steps:

1. Go to your console's device menu. For more information, see [Navigating to devices](/docs/vsi?topic=virtual-servers-navigating-devices).
2. From the **Devices** menu, select **Device List** and select the device.
3. Click the **Monitoring** tab. All current pings are viewable on the landing page. 

## Getting started with Sysdig

For information about setting up a Sysdig IBM Cloud monitoring agent, see [Getting started with Sysdig](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-getting-started).

The **Monitoring** tab is only visible if at least one monitor is configured.
{:note}

