---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 建立及管理監視通知（測試版）
通知會說明在觸發警示時用來通知的方法及詳細資料。例如，若要取得度量值的警告通知及錯誤通知，請定義一個監視警告臨界值的規則，以及定義一個監視錯誤臨界值的規則。
{:shortdesc}

## 建立通知

 1. 在您加入了測試版之後，選取**裝置 -> 監視**。
 2. 按一下**通知**標籤。
 3. 按一下**建立通知**。
 4. 輸入新通知的資訊。

<table>
  <caption>電子郵件通知詳細資料</caption>
  <tr>
     <th>欄位</th>
     <th>說明</th>
  </tr>
  <tr>
    <td>名稱</td>
    <td>通知的唯一 ID。這是必要欄位。</td>
  </tr>
  <tr>
    <td>類型</td>
    <td>選取：**電子郵件**</td>
  </tr>
  <tr>
    <td>電子郵件位址</td>
    <td>輸入收件者的電子郵件位址。</td>
  </tr>
</table>

<table>
  <caption>Webhook 通知詳細資料</caption>
  <tr>
     <th>欄位</th>
     <th>說明</th>
  </tr>
  <tr>
    <td>名稱</td>
    <td>通知的唯一 ID。這是必要欄位。</td>
  </tr>
  <tr>
    <td>類型</td>
    <td>選取：**Webhook**</td>
  </tr>
  <tr>
    <td>Webhook URL</td>
    <td>輸入應該進行 POST 的 URL。</td>
  </tr>
  <tr>
  <td>驗證憑證</td>
    <td>選取以驗證憑證。</td>
  </tr>
  <tr>
    <td>Webhook 標頭</td>
    <td>輸入任何標頭。</td>
  </tr>
  <tr>
    <td>Webhook 查詢參數</td>
    <td>輸入任何查詢參數。</td>
  </tr>
</table>

<table>
  <caption>值班 (pager duty) 通知詳細資料</caption>
  <tr>
     <th>欄位</th>
     <th>說明</th>
  </tr>
  <tr>
    <td>名稱</td>
    <td>通知的唯一 ID。這是必要欄位。</td>
  </tr>
  <tr>
    <td>類型</td>
    <td>選取：**值班**</td>
  </tr>
  <tr>
    <td>API 金鑰</td>
    <td>輸入值班通知的「API 金鑰」。</td>
  </tr>
</table>


5. 按一下**確定**，使用您指定的設定來建立新通知。

## 編輯通知
 1. 在您加入了測試版之後，選取**裝置 -> 監視**。
 2. 按一下**通知**標籤。
3. 按一下**動作->編輯通知**。
4. 編輯任何通知詳細資料。
5. 按一下**確定**以接受您的變更。

## 刪除通知
1. 在您加入了測試版之後，選取**裝置 -> 監視**。
2. 按一下**通知**標籤。
3. 按一下**動作->刪除通知**。
4. 按一下**刪除**以確認您的選擇。

## 將多個通知新增至裝置
1. 選取**基礎架構->裝置清單->*裝置名稱***，以存取裝置詳細資料。
2. 按一下**動作->管理通知**。
4. 按一下以指派或移除裝置的通知。
