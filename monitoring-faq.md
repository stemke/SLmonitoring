---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

# FAQs
{: #monitoring-faq}

## I'm seeing numerous monitoring alert tickets. Does this mean that my server is down?
{: faq}

Each device comes with a complimentary monitoring ping and notify service. This service automatically creates a monitoring alert ticket upon failing set parameters. False positives are possible with the monitoring service and can be attributed to rate limiting by a software firewall on the server, service and application availability, and service interruptions within the monitoring infrastructure. Review the default settings to mitigate possible false monitoring alerts.

## Can I have the monitoring system issue an automatic reboot and alert a support technician if the server stops responding?
{: faq}

Yes, with the **Automated Reboot from Monitoring Failure** service, you can set up the monitoring system to automatically reboot the server and issue a ticket for a support technician if a monitoring alert is issued.

## What is the difference between monitoring with a “slow ping” and a “service ping”?
{: faq}

The difference between a service ping and a slow ping is the amount of time in which a response from a device is expected. The default is the service ping, but you can change to use a slow ping, instead.

* A **service** ping issues one ping every 5 minutes and expects an echo reply within 1 second. If more than one ping is missed, an alert is issued.
* A **slow** ping waits 5 seconds for a reply, allowing servers that are optimized for non-network tasks more time to process the request.


## When a monitoring ticket is opened and alerts me to the issue, will the technicians see the ticket and respond?
{: faq}

With the basic ping service, support technicians aren't notified of failures. These tickets are opened when the monitoring system issues an alert, and they notify only the users that you specify on the monitoring screen. Technicians aren't alerted until you open a new ticket stating that the server is not responding.


## When a monitoring ticket is opened and alerts me to the issue, will the technicians see the ticket and respond?
{: faq}

With the basic ping service, support technicians aren't notified of failures. These tickets are opened when the monitoring system issues an alert, and they notify only the users that you specify on the monitoring screen. Technicians aren't alerted until you open a new ticket stating that the server is not responding.
