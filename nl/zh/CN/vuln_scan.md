---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-02"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 漏洞扫描
{{site.data.keyword.BluSoftlayer_full}} 与 Nessus 合作为 {{site.data.keyword.BluSoftlayer_notm}} 网络上的任何设备提供漏洞扫描。漏洞扫描会测试设备中的薄弱区域，并返回有关主机设备的分析、安全问题和修订的报告。在设备上执行漏洞扫描可确保设备始终保持安全，当您认为设备可能受到攻击或威胁时，也可以首先查看漏洞扫描报告来确定是否存在安全问题。通过 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}，可以在与帐户相关联的任何设备上完成漏洞扫描。
{:shortdesc}

## Nessus 安全性扫描程序
{{site.data.keyword.BluSoftlayer_notm}} 提供了基于开放式源代码 Nessus 扫描工具的联机安全性扫描程序。通过单击**扫描程序**，可以在“安全”选项卡下访问此安全性扫描程序。有关更多信息，请参阅 [Nessus 扫描工具 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://www.nessus.org/nessus/){: new_window}。

**扫描程序**页面提供了适用于 {{site.data.keyword.BluSoftlayer_notm}} 托管的 Nessus 工具的硬件列表。要扫描服务器或查看先前扫描的结果，请单击要检查的服务器的详细信息链接。漏洞扫描详细信息页面会显示服务器的简短摘要（包括服务器名称、要扫描的 IP 地址以及服务器所在的数据中心）。**启动扫描**会安排 Nessus 扫描服务器尽快对您的服务器进行漏洞扫描。

服务器摘要之后是一个显示当前和过去 Nessus 漏洞扫描的表格。其中分别列出了每个扫描的扫描请求日期、扫描启动日期和扫描状态，如果扫描已完成，还会列出 Nessus 报告的链接。

Nessus 报告可以是以下某个状态：

* 扫描暂挂：已安排 Nessus Scanner Box 执行扫描。
* 正在扫描：当前正在进行扫描。
* 正在生成报告：已完成扫描，正在将测试结果编译成报告。
* 扫描完成：已成功完成扫描，并已生成漏洞报告。
* 扫描已取消：{{site.data.keyword.BluSoftlayer_notm}} 技术人员已手动取消 Nessus 扫描。

要查看此表中列出的所有成功完成的 Nessus 扫描，可通过单击**查看报告**来查看报告。报告包含两个表：扫描详细信息表，其中列出已扫描的主机数、已找到的未解决的安全漏洞数以及已找到的可能的安全漏洞数（警告）。第二个表列出了所有找到的安全问题：在哪个主机上找到了漏洞以及对可能漏洞的描述。

开放式源代码 Nessus 工具是基于插件的，支持在找到漏洞时开发新测试。{{site.data.keyword.BluSoftlayer_notm}} 会定期更新内部 Nessus 工具，因此建议使用安全性扫描程序定期进行扫描，以免受最新威胁的攻击。

为确保扫描成功，需要允许来自 173.192.255.232 和 172.17.19.38 的连接访问您的服务器。
