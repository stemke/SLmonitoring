---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring, Nimsoft

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Getting started tutorial
{: #monitoring}

{{site.data.keyword.cloud}} offers both standard monitoring services and Nimsoft Monitoring to ensure that you're always aware of any issues with your devices. Standard monitoring services include features like Ping and IPMI Statistics. Nimsoft Monitoring consists of three levels of monitoring, including basic, advanced, and premium monitoring. Each service within both standard and Nimsoft Monitoring offerings features various benefits and are available at various pricing options to meet your business needs. For more information, see  [{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}.
{:shortdesc}

Monitoring a device allows you to initiate service and slow pings to ensure that the device is online and responsive.

If an echo isn't received in the allotted time frame (1 second for service pings, 5 seconds for slow pings) an alert is sent to the email address on the account. A status of **Up** in the **Status** field indicates that an echo was received, while **Down** indicates that the echo wasn't received.

To view configured monitors, follow these steps:

1. Navigate to your console's device menu. For more information, see [Navigating to devices](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
2. From the **Devices** menu, select **Device List** and select the device.
3. Click the **Monitoring** tab. All current pings are viewable on the landing page. 

The **Monitoring** tab is only visible if at least one monitor is configured.
{:note}

