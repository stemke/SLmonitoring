---
copyright:
  years: 2018
lastupdated: "2018-05-18"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 创建和管理监视通知 (Beta)
通知描述了在触发警报时用作通知内容的方法和详细信息。例如，要获取某个度量值的警告通知和错误通知，请定义一个规则来监视警告阈值，再定义一个规则来监视错误阈值。
{:shortdesc} 

## 创建通知
 
 1. 在加入 Beta 后，选择**设备 -> 监视**。 
 2. 单击**通知**选项卡。
 3. 单击**创建通知**。
 4. 输入新通知的信息。 

<table>
  <caption>电子邮件通知详细信息</caption>
  <tr>
     <th>字段</th>
     <th>描述</th>
  </tr>
  <tr>
    <td>名称</td>
    <td>通知的唯一标识。此为必填字段。</td>
  </tr>
  <tr>
    <td>类型</td>
    <td>选择：**电子邮件**</td>
  </tr>
  <tr>
    <td>电子邮件地址</td>
    <td>输入接收方的电子邮件地址。</td>
  </tr>
</table>

<table>
  <caption>Webhook 通知详细信息</caption>
  <tr>
     <th>字段</th>
     <th>描述</th>
  </tr>
  <tr>
    <td>名称</td>
    <td>通知的唯一标识。此为必填字段。</td>
  </tr>
  <tr>
    <td>类型</td>
    <td>选择：**Webhook**</td>
  </tr>
  <tr>
    <td>Webhook URL</td>
    <td>输入应在哪个 URL 上执行 POST 操作。</td>
  </tr>
  <tr>
  <td>验证证书</td>
    <td>选择以验证证书。</td>
  </tr>
  <tr>
    <td>Webhook 头</td>
    <td>输入任何头。</td>
  </tr>
  <tr>
    <td>Webhook 查询参数</td>
    <td>输入任何查询参数。</td>
  </tr>
</table>

<table>
  <caption>Pager duty 通知详细信息</caption>
  <tr>
     <th>字段</th>
     <th>描述</th>
  </tr>
  <tr>
    <td>名称</td>
    <td>通知的唯一标识。此为必填字段。</td>
  </tr>
  <tr>
    <td>类型</td>
    <td>选择：**Pager duty**</td>
  </tr>
  <tr>
    <td>API 密钥</td>
    <td>输入 Pager duty 通知的 API 密钥。</td>
  </tr>
</table>


5. 单击**确定**，以使用指定的设置来创建新通知。

## 编辑通知
 1. 在加入 Beta 后，选择**设备 -> 监视**。 
 2. 单击**通知**选项卡。
3. 单击**操作 -> 编辑通知**。
4. 编辑任何通知详细信息。
5. 单击**确定**以接受更改。

## 删除通知
1. 在加入 Beta 后，选择**设备 -> 监视**。 
2. 单击**通知**选项卡。
3. 单击**操作 -> 删除通知**。
4. 单击**删除**以确认您的选择。

## 向设备添加多个通知
1. 选择**基础架构 -> 设备列表 -> *设备名称***以访问设备详细信息。
2. 单击**操作 -> 管理通知**。
4. 单击以分配或除去设备的通知。

