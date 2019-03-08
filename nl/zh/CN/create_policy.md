---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 创建和管理系统策略 (Beta)
您可以创建策略以在设备达到预先确定的监视阈值时触发通知。例如，可以在设备的平均 CPU 使用率达到警告或错误级别时通知用户。仅允许 10 个监视策略同时存在。不过，可以将一个策略应用于多个设备。
{:shortdesc}


要使用系统策略，请执行以下操作。
1. 在加入 Beta 后，选择**设备 -> 监视**。
2. 单击**系统策略**选项卡。

<table>
   <CAPTION>表 1. 创建和管理系统策略</CAPTION>
   <THEAD>
   <TR>
   <th>如果要执行的操作是...</th>
   <th>请执行以下操作...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>创建策略</td>
   <td>
   <ol>
     <li>单击<b>创建通知</b>。</li>
     <li>输入新系统策略的信息。

<table>
  <caption>系统策略详细信息</caption>
  <tr>
     <th>字段</th>
     <th>描述</th>
  </tr>
  <tr>
    <td>名称</td>
    <td>输入新系统策略的唯一标识。此为必填字段。</td>
  </tr>
  <tr>
    <td>触发器</td>
    <td>选择用于触发系统策略的详细信息。对于警告和错误，此项可以是不同的度量值级别。例如，<i>平均值</i>。</td>
  </tr>
   <tr>
    <td>持续时间</td>
     <td>选择在事件发生后多长时间会触发策略。</td>
  </tr>
   <tr>
    <td>设备</td>
    <td>策略所应用到的受监视设备。</td>
  </tr>
   <tr>
    <td>缺省通知</td>
    <td>定义策略的缺省通知。</td>
  </tr>
</table>
</li>
<li>单击<b>确定</b>以接受更改。</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>编辑策略</td>
   <td>
   <ol>
     <li>单击<b>编辑策略</b>。</li>
    <li>输入系统策略的更改信息。

<table>
  <caption>系统策略详细信息</caption>
  <tr>
     <th>字段</th>
     <th>描述</th>
  </tr>
  <tr>
    <td>名称</td>
    <td>输入新系统策略的唯一标识。此为必填字段</td>
  </tr>
  <tr>
    <td>触发器</td>
    <td>选择用于触发系统策略的详细信息。对于警告和错误，此项可以是不同的度量值级别。</td>
  </tr>
   <tr>
    <td>持续时间</td>
     <td>选择在事件发生后多长时间会触发策略。</td>
  </tr>
</table>
</li>
<li>单击<b>确定</b>以接受更改。</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>除去策略</td>
   <td>
   <ol>
     <li>单击<b>操作 -> 删除策略</b>。</li>
     <li>单击<b>删除</b>以确认您的选择。</li>
   </ol>
   </td>
   </tr>
   <tr>
  <td>分配设备</td>
  <td>
    <ol>
      <li>单击<b>管理设备</b>。</li>
      <li>选择或取消选择要为其分配策略的设备。</li>
       <li>单击<b>确定</b>以接受更改。</li>
    </ol>
      </td>
  </tr>
   <tr>
  <td>复制策略</td>
  <td>
    <ol>
      <li>单击<b>操作 -> 复制策略</b>。</li>
      <li>输入新策略的任何更改信息。</li>
       <li>单击<b>确定</b>以接受更改。</li>
    </ol>
      </td>
  </tr>

   </TBODY>
   </table>
