---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 管理标准监视的通知用户
{: #managing-notified-users-for-standard-monitoring}

如果设备未在分配的响应时间内响应 ping，那么标准监视服务的通知用户会收到系统自动发送的通知。您可以随时添加或除去通知用户，并且通知用户必须位于与设备相关联的帐户上才能接收通知。要管理标准监视服务的通知用户，请执行以下步骤。
{:shortdesc}

## 开始之前
首先，导航至设备菜单，并确保您有正确的帐户许可权来完成任务。

* 导航至控制台的设备菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)。
* 确保您有任何必要的帐户许可权和设备访问权。仅帐户所有者或具有**管理用户**经典基础架构许可权的用户可以调整许可权。

有关许可权的更多信息，请参阅[经典基础架构许可权](/docs/iam?topic=iam-infrapermission#infrapermission)和[管理设备访问权](/docs/vsi?topic=virtual-servers-managing-device-access)。

## 添加通知用户
{: #adding-notified-users}

要添加标准监视服务的通知用户，请完成以下步骤。
1. 从**设备**菜单中，选择**设备列表**。
2. 单击设备名称以访问该设备。
3. 单击**监视**选项卡，然后选择**管理监视器**。
4. 选择**管理通知用户**。
5. 从**要通知的用户**下拉列表中，选择要通知的新用户。
6. 选择**添加用户**。

## 除去通知用户
{: #removing-notified-users}

要除去标准监视服务的通知用户，请完成以下步骤。
1. 从**设备**菜单中，选择**设备列表**。
2. 单击设备名称以访问该设备。
3. 单击**监视**选项卡，然后选择**管理监视器**。
4. 选择**管理通知用户**。
5. 单击**除去**图标以除去现有通知用户，然后选择**是**以除去用户。 

## 后续步骤

如果添加了通知用户，那么会在没有 ping 响应时通知该用户。如果除去了通知用户，那么该用户将不会再收到与没有 ping 响应（与设备相关联）相关的通知。
