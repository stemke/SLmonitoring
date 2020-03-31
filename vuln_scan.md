---

copyright:
  years: 2014, 2020
lastupdated: "2020-03-31"

keywords: Nessus, Security, Nessus Security Scanner, scanner, vulnerability

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# Vulnerability scans
{: #vulnerability-scans}

{{site.data.keyword.cloud}} works with Nessus to provide vulnerability scans for any device on the {{site.data.keyword.cloud_notm}} network. Vulnerability scans test for areas of weakness in a device and return a report of the analysis, security issues, and fixes for your host device. Running vulnerability scans on your devices make sure that they always stay secure and are also the first resource to employ when you think a device might be vulnerable or compromised. Vulnerability scans can be completed by using the {{site.data.keyword.cloud_notm}} console on any device that is associated with your account that has a public IP address. If the device is private network only, vulnerability scans can't be done.
{:shortdesc}

## Nessus Security Scanner
{{site.data.keyword.cloud_notm}} provides an online security scanner, which is powered by the open source Nessus Scanning tool. This security scanner can be accessed under the Security tab by clicking **Scanner**. For more information, see [Nessus Scanning tool](http://www.nessus.org/nessus/){: external}.

The **Scanner** page provides a list of hardware that is available to the Nessus tool hosted by {{site.data.keyword.cloud_notm}}. To scan a server, or to see the results of a previous scan, click the details link for the server that you want to inspect. The vulnerability scanning details page shows a short summary of the server. The summary includes the server name, the IP address that to be scanned, and the server data center. **Start Scan** schedule your server with the Nessus scanning server to be scanned for vulnerabilities as soon as possible.

After the server summary is a table of current and past Nessus vulnerability scans that gives you the following information: 
* The date that the scan was requested 
* The date that the scan was started 
* The status of the scan and whether the scan is complete 
* A link to the Nessus report

Nessus reports can have one of these statuses:

* Scan Pending: The scan is scheduled for the Nessus scanner box.
* Scan Processing: The scan is in progress.
* Generating Report: The scan is complete and test results are compiling into a report.
* Scan Complete: The scan completed successfully and the vulnerability report was generated.
* Scan Canceled: The Nessus scan was manually canceled by a {{site.data.keyword.cloud_notm}} technician.

For all successfully completed Nessus scans listed in this table, a report can be viewed by clicking **View Report**. The report has two tables: 
- The **Scan Details** table lists the number of scanned hosts, the number of open security vulnerabilities (holes) found, and the number of possible security vulnerabilities (warnings) found. 

- The second table lists all the security issues found: the host that the vulnerability was found on, and a description of the possible vulnerability.

The open source Nessus tool is plug-in based, which allows new tests to be developed as vulnerabilities are found. {{site.data.keyword.cloud_notm}} updates the internal Nessus tool regularly, so regular scanning with the security scanner is recommended to keep up to date with new threats.

For a successful scan, connections from `169.48.118.71`, `173.192.255.232`, `172.17.19.38`, and `172.22.211.38` need to be allowed access to your server.
