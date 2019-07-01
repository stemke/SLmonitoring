---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 入门教程
{: #monitoring}

为了确保您始终都能了解设备发生的任何问题，{{site.data.keyword.cloud}} 提供了标准监视服务和 Nimsoft 监视。标准监视服务包括 Ping 和 IPMI 统计信息等功能。Nimsoft 监视服务由三个级别的监视组成：基本监视、高级监视和特级监视。标准监视服务和 Nimsoft 监视服务中的每项服务都具有不同的优点，并以不同的定价选项提供，可满足您的各种业务需求。有关更多信息，请参阅 [{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}。
{:shortdesc}

通过监视设备，您可以启动服务 ping 和慢速 ping 来确保设备处于联机状态并且可进行响应。

如果在分配的时间范围（服务 ping 为 1 秒，慢速 ping 为 5 秒）内未收到回送信号，那么会向帐户上的电子邮件地址发送警报。在**状态**字段中，若显示**已启动**状态，则指示已收到回送信号；若显示**已关闭**状态，则指示还未收到回送信号。

要查看配置的监视器，请执行以下步骤：

1. 导航至控制台的设备菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)。
2. 从**设备**菜单中，选择**设备列表**，然后选择设备。
3. 单击**监视**选项卡。所有当前 ping 都可在登录页面上进行查看。 

仅当至少配置了一个监视器时，**监视**选项卡才会显示。
{:note}

