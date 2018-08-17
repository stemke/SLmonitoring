---



copyright:
  years: 2014, 2017
lastupdated: "2017-11-01"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 监视
为了确保您始终都能了解设备发生的任何问题，{{site.data.keyword.BluSoftlayer_full}} 提供了标准监视服务和 Nimsoft 监视服务。标准监视服务包括 Ping 和 IPMI 统计信息等功能。Nimsoft 监视服务由三个级别的监视组成：基本监视、高级监视和特级监视。标准监视服务和 Nimsoft 监视服务中的每项服务都具有不同的优点，并以不同的定价选项提供，可满足您的各种业务需求。有关更多信息，请参阅 [{{site.data.keyword.cloud}} 基础架构监视和报告](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}。

通过监视设备，用户可以启动服务 ping 和慢速 ping 来确保设备处于联机状态并且可进行响应。

如果在分配的时间范围（服务 ping 为 1 秒，慢速 ping 为 5 秒）内未收到回送信号，那么会向帐户上的电子邮件地址发送警报。在**状态**字段中，若显示**已启动**状态，则指示收到回送信号；若显示**已关闭**状态，则指示未收到回送信号。 

要查看配置的监视器，请执行以下步骤：

1\. 在“设备列表”中，单击**设备名称**以访问该设备。

2\. 单击**监视**选项卡。所有当前 ping 都可在登录页面上进行查看。（必须至少有一个配置的监视器，才会显示**监视**选项卡。）



