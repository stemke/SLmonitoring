---
copyright:
  years: 2014, 2019
lastupdated: "2019-02-11"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installing and managing the Nimsoft Monitoring Robot

To allow advanced monitoring to function on existing {{site.data.keyword.baremetal_short}} or {{site.data.keyword.BluVirtServers_short}}, install the Nimsoft Monitoring Robot. The Nimsoft Monitoring Robot allows the monitoring management system to communicate with the bare metal server or virtual server on the private network. After you install the Nimsoft Monitoring Robot, it takes approximately 5 - 10 minutes to become available on the {{site.data.keyword.slportal_full}}. Follow these steps to install the Nimsoft Monitoring Robot in Windows or Linux.

## Prerequisites

Before you install, these ports must be open on the private network:

* tcp/48000
* tcp/48001
* tcp/48002

Additionally, open ports tcp/48003 through tcp/50000 for the private network to allow for full functionality that is used by the API. If you do not open these ports, some monitoring agents are affected. If errors are encountered during configuration, ensure that these ports are open before you open a ticket for escalation. 

* **openjdk** is required for certain monitoring agents, such as the Tomcat Monitoring Agent.
* Some 64-bit Linux distributions require **glibc.i686** and **nss-softtokn-freebl.i686**.
* The monitoring system is not supported in **FreeBSD**.

If there is an error configuring the monitoring service due to communication errors with the Nimsoft robot, the configuration process can be paused due to the limited connectivity. Limited connectivity is often caused by firewall or other security software that is blocking access to the system from the Nimsoft management servers.  Follow these steps to restart provisioning of the monitoring service:

## Restarting provisioning of a monitoring agent

1. Go to the **Devices** menu, and select **Monitoring**.
* Find the system for which monitoring is being configured.
* Select **"Redeploy all agents"** under the **Advanced** drop-down in the right column.
* Choose a monitoring template on the **Pop-In** page.
* Click **Re-Deploy**

## Installing in Windows

1. See http://downloads.service.softlayer.com/nimsoft/ to download the latest version of the Windows Installer to the device for installation (You must be connected to the customer VPN).
* Run the Nimsoft Monitoring Robot file as an Administrator.

## Installing in Linux

1. Connect to the private network through the customer VPN.
* Download the [32-bit ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} or [64-bit ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} Linux Installer to the device for installation. Debian and Ubuntu versions are also available on the [Nimsoft Installer ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://downloads.service.softlayer.com/nimsoft/){: new_window}.
* Run these commands to complete the installation, replacing 32 with 64, if you are running a 64-bit installation:

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Next steps

After you run the installation, the system automatically completes the process. In Windows, a message appears with a confirmation of a successful install or with information about any errors that occurred.
