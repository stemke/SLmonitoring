---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 查看 Nimsoft 监视的代理程序报告
{: #viewing-an-agent-report-for-nimsoft-monitoring}

有关 Nimsoft 监视的监视详细信息，可查看代理程序报告，其中提供了特定于代理程序配置方式的详细信息。
{:shortdesc}

## 开始之前
首先，导航至设备菜单，并确保您有正确的帐户许可权来完成任务。

* 导航至控制台的设备菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)。
* 确保您有任何必要的帐户许可权和设备访问权。仅帐户所有者或具有**管理用户**经典基础架构许可权的用户可以调整许可权。

有关许可权的更多信息，请参阅[经典基础架构许可权](/docs/iam?topic=iam-infrapermission#infrapermission)和[管理设备访问权](/docs/vsi?topic=virtual-servers-managing-device-access)。

## 查看 Nimsoft 监视的代理程序报告
{: #viewing-agent-report-nimsoft-monitoring-steps}

要查看 Nimsoft 监视的代理程序报告，请完成以下步骤。

1. 在**监视**页面上，从**操作**菜单中选择**查看代理程序报告**。
2. 从**代理程序**列表中选择要查看的代理程序。

  可用的代理程序因设备而异，并且取决于应用于设备的监视包。
  {:note}
  
3. 完成所有剩余部分，包括一个或多个以下操作：

  所显示内容因代理程序而异，并非每个部分或度量值都会显示。此屏幕上的可用选项取决于适用于每个代理程序的配置选项。
  {:note}
  
  * 从**部分**列表中选择部分报告。
  * 从**查看依据**列表中选择报告的时间段。
  * 在**选择要报告的度量值：**部分中，单击要包含在报告中的每个度量值的复选框。
    
    只有类似的度量值会显示在同一图形上。如果所选度量值有冲突，那么在请求图形后会发生错误。
    {:note}
4. 单击**绘制图形**以绘制图形。

## 后续步骤

在针对代理程序报告绘制图形后，可随时通过重复上述步骤来重新绘制图形，以查看不同的度量值。一段时间内可生成的代理程序报告数是没有限制的。
