---

copyright:
  years: 2018
lastupdated: "2018-04-20"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installing IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)
{: #install-service}

To allow advanced monitoring to function on existing {{site.data.keyword.baremetal_short}}, follow these steps to install the {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent on your bare metal device.

## Prerequisites
You must be connected to your bare metal device to download and run the installers.

## Installing in Windows

1. Download the Windows IBM Cloud Monitoring Agent installer. [Download ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi){: new_window}
2. Run the installer on the target machine.

## Installing in Linux

1. Download the Linux IBM Cloud Monitoring Agent installer. [Download ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz){: new_window}
2. Extract it on the target machine.
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. Run the linux_install.sh script.


## Installing in FreeBSD
1. Download the FreeBSD IBM Cloud Monitoring Agent installer. [Download ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz){: new_window}
2. Extract it on the target machine.
       `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. Run the freebsd_install.sh script.

## Next steps

After you run the installation, the system automatically completes the process. In Windows, a message appears with a confirmation of a successful install or with information about any errors that occurred.

If you're using a firewall, you might need to allow the IBM Cloud Monitoring Agent to pass data through it. The agent uses port 8090 for outbound HTTPS communication. For more information on IP addresses you might need to allow, see [Load balancer IP ranges](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-load-balancer-ips#load-balancer-ips).
