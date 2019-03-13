---

copyright:
  years: 2014, 2018
lastupdated: "2018-11-15"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Monitoring
{: #monitoring}

{{site.data.keyword.BluSoftlayer_full}} offers both Standard Monitoring Services and Nimsoft Monitoring to ensure that you're always aware of any issues with your devices. Standard Monitoring Services include features like Ping and IPMI Statistics. Nimsoft Monitoring consists of three levels of monitoring, including basic, advanced, and premium monitoring. Each service within both Standard and Nimsoft Monitoring offerings features various benefits and are available at various pricing options to meet your business needs. For more information, see  [{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}.

Monitoring a device allows users to initiate service and slow pings to ensure that the device is online and responsive.

If an echo isn't received in the allotted time frame (1 second for service pings, 5 seconds for slow pings) an alert is sent to the email
address on the account. A status of **Up** in the **Status** field indicates that an echo was received, while **Down**
indicates that the echo wasn't received.

To view configured monitors, follow these steps:

1. From the Device List, click the **Device Name** to access the device.

2. Click the **Monitoring** tab. All current pings are viewable on the landing page. (The **Monitoring** tab is only visible if at least one monitor is configured.)
