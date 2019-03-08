---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 建立及管理系統原則（測試版）
您可以建立原則，以在裝置達到預先決定的監視臨界值時觸發通知。比方說，如果裝置的平均 CPU 使用率達到警告或錯誤層次，則您可以通知使用者。一次只能存在 10 個監視原則。不過，一個原則可以套用至多個裝置。
{:shortdesc}


請遵循下列步驟以使用您的系統原則。
1. 在加入測試版之後，選取**裝置 -> 監視**。
2. 按一下**系統原則**標籤。

<table>
   <CAPTION>表 1. 建立及管理系統原則</CAPTION>
   <THEAD>
   <TR>
   <th>如果要採取的動作是...</th>
   <th>則...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>建立原則</td>
   <td>
   <ol>
     <li>按一下<b>建立通知</b>。</li>
     <li>輸入新系統原則的資訊。

<table>
  <caption>系統原則詳細資料</caption>
  <tr>
     <th>欄位</th>
     <th>說明</th>
  </tr>
  <tr>
    <td>名稱</td>
    <td>輸入新系統原則的唯一 ID。這是必要欄位。</td>
  </tr>
  <tr>
    <td>觸發</td>
    <td>選取觸發系統原則的詳細資料。對於警告及錯誤，這可以是不同的度量值層次。例如，<i>平均值</i>。</td>
  </tr>
   <tr>
    <td>持續時間</td>
     <td>選取發生事件以觸發原則的時間長度。</td>
  </tr>
   <tr>
    <td>裝置</td>
    <td>針對原則所監視的裝置。</td>
  </tr>
   <tr>
    <td>預設通知</td>
    <td>定義原則的預設通知。</td>
  </tr>
</table>
</li>
<li>按一下<b>確定</b>以接受您的變更。</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>編輯原則</td>
   <td>
   <ol>
     <li>按一下<b>編輯原則</b>。</li>
    <li>輸入系統原則的已變更資訊。

<table>
  <caption>系統原則詳細資料</caption>
  <tr>
     <th>欄位</th>
     <th>說明</th>
  </tr>
  <tr>
    <td>名稱</td>
    <td>輸入新系統原則的唯一 ID。這是必要欄位</td>
  </tr>
  <tr>
    <td>觸發</td>
    <td>選取觸發系統原則的詳細資料。對於警告及錯誤，這可以是不同的度量值層次。</td>
  </tr>
   <tr>
    <td>持續時間</td>
     <td>選取發生事件以觸發原則的時間長度。</td>
  </tr>
</table>
</li>
<li>按一下<b>確定</b>以接受您的變更。</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>移除原則</td>
   <td>
   <ol>
     <li>按一下<b>動作->刪除原則</b>。</li>
     <li>按一下<b>刪除</b>以確認您的選擇。</li>
   </ol>
   </td>
   </tr>
   <tr>
  <td>指派裝置</td>
  <td>
    <ol>
      <li>按一下<b>管理裝置</b>。</li>
      <li>選取或取消選取要指派原則的裝置。</li>
       <li>按一下<b>確定</b>以接受您的變更。</li>
    </ol>
      </td>
  </tr>
   <tr>
  <td>複製原則</td>
  <td>
    <ol>
      <li>按一下<b>動作->複製原則</b>。</li>
      <li>輸入新原則的任何已變更資訊。</li>
       <li>按一下<b>確定</b>以接受您的變更。</li>
    </ol>
      </td>
  </tr>

   </TBODY>
   </table>
