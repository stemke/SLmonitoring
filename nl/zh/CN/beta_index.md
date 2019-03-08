---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# IBM Cloud Monitoring (Beta) 入门
{: #gettingstartedbeta}

此 Beta 监视应用程序基于 {{site.data.keyword.BluSoftlayer_full}} Monitoring Service 构建，可用于虚拟服务器和裸机服务器。有关此 Beta 程序开发的更新内容，请参阅 [IBM Cloud 博客 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}。{:shortdesc}

## 先决条件

要参与此 Beta 程序，必须满足以下需求。
1. SoftLayer 帐户必须通过 IBM 标识认证链接到 IBM Cloud 帐户。要链接帐户，SoftLayer 帐户的“主用户”必须登录到 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com){: new_window}，然后单击**帐户**菜单中的**链接 Bluemix 帐户！**。
2. 每个要查看 Beta 的用户都必须链接到一个 IBM 标识。有关更多信息，请参阅[链接 IBM 标识用户帐户](/docs/account?topic=account-unifyingaccounts#link_customer_accounts)。
3. 每个要查看 Beta 的用户都必须具有 IBM Cloud Monitoring Service 访问权。
   1. 从 [IBM Cloud 控制台 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://console.bluemix.net){: new_window} 中，选择**管理 -> 帐户 -> 用户**。
   2. 邀请用户加入帐户，或从列表中选择用户。
   3. 选择**分配对资源的访问权**，向用户分配访问权。
   4. 从**服务**中，选择 **IBM Cloud Monitoring Service**。
   5. 针对所有区域，选择要授予给用户的**角色**。

如果不满足上述先决条件，那么此时无法访问 Beta 监视。


## 加入 Beta

要开始使用监视 Beta 程序，请执行以下步骤。加入 Beta 可以为您帐户中所有符合条件的虚拟服务器和裸机服务器启用此服务。单击“加入”不会影响现有 Nimsoft 监视或数据。
1. （仅限裸机）[在裸机服务器上安装监视代理程序](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-)。
<table>
   <CAPTION>表 1. 选择登录位置</CAPTION>
   <THEAD>
   <TR>
   <th>如果想要使用以下方式加入...</th>
   <th>请执行以下操作...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>IBM Cloud 目录</td>
   <td>
   <ol>
   <li>打开新的浏览器窗口，然后输入 <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>。</li>
   <li>单击<b>登录</b>链接。</li>
   <li>输入您的电子邮件或 IBM 标识，然后单击<b>继续</b>。</li>
   <li>输入您的密码，然后单击<b>登录</b>。</li>
   <li>选择**基础架构 -> 设备列表 -> *设备名称***以访问设备详细信息。</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>客户门户网站</td>
   <td>
   <ol>
   <li>打开新的浏览器窗口，然后输入 <a href="https://control.softlayer.com">https://control.softlayer.com</a>。</li>
   <li>键入用户名和密码，然后单击<b>登录</b>。或者，单击<b>使用 IBM 标识登录</b>。接下来，输入您的电子邮件或 IBM 标识，然后单击<b>继续</b>。输入您的密码，然后单击<b>登录</b>。这将打开 {{site.data.keyword.slportal}} 的主页面。</li>
     <li>在**设备**中，单击**设备名称**以访问设备详细信息。</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. 选择**设备 -> 监视**。单击**加入 Beta** 以查看系统策略和通知 Beta 选项卡。

## 后续步骤
1. 查看所收集的[度量值](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-)的详细信息。
2. [创建或管理](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-)监视通知。
3. [创建或管理](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-)系统策略。
4. [查看警报](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-)。
5. 查看所选设备的当前可用 Beta 监视图形数据。

|              度量值                                       |  描述                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU 使用率|   查看每个核心的 % CPU 使用率和所有核心的平均值。单击键中的每个度量值，可在图形上打开或关闭数据。
|公用网络                                             |   查看公用网络的入站和出站数据。单击键中的每个度量值，可在图形上打开或关闭数据。
|
|专用网络                                            |   查看专用网络的入站和出站数据。单击键中的每个度量值，可在图形上打开或关闭数据。
|
|内存利用率| 查看服务器的内存利用率 %      |
|磁盘使用情况|查看从磁盘读取或写入磁盘的平均数据量（以字节为单位）或磁盘等待时间。单击键中的每个度量值，可在图形上打开或关闭数据。
|
|温度|查看裸机设备的温度，以摄氏度为单位。此数据并非适用于所有设备。
{: caption="表 1. Beta 度量值" caption-side="top"}   

## 限制
删除设备并不会删除关联的监视策略。请注意，必须手动删除设备的这些策略。

仅会将度量值数据保留 15 天。

仅允许 10 个监视策略同时存在。不过，可以将一个策略应用于多个设备。

## 故障诊断
要查看某些度量值（如内存利用率），需要在服务器上安装 Xen 工具。有关安装 Xen 工具的信息，请参阅[准备和导入映像](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images)。

## 反馈
要提供有关此 Beta 的反馈，请选择**设备 -> 监视**或设备详细信息页面，然后单击**留下反馈**以完成简短的调查。要离开 Beta 而返回至标准视图，请单击**设备 -> 监视**页面底部的**离开 Beta** 链接。
