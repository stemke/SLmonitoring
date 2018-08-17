---
copyright:
  years: 2018
lastupdated: "2018-05-18"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# モニター通知の作成および管理 (ベータ)
通知には、アラートがトリガーされたときに通知する方法と詳細を記述します。例えば、あるメトリックについて警告通知とエラー通知を受け取るには、警告しきい値をモニターするルールを定義し、エラーしきい値をモニターするルールを定義します。{:shortdesc} 

## 通知の作成
 
 1. ベータ版に参加した後、**「デバイス」-> 「モニタリング」**を選択します。 
 2. **「通知」**タブをクリックします。
 3. **「通知の作成 (Create Notification)」**をクリックします。
 4. 新しい通知の情報を入力します。 

<table>
  <caption>E メール通知の詳細</caption>
  <tr>
     <th>フィールド</th>
     <th>説明</th>
  </tr>
  <tr>
    <td>名前</td>
    <td>通知の固有 ID。このフィールドは必須です。</td>
  </tr>
  <tr>
    <td>タイプ </td>
    <td>**「E メール」**を選択します。</td>
  </tr>
  <tr>
    <td>E メール・アドレス</td>
    <td>受信者の E メール・アドレスを入力します。</td>
  </tr>
</table>

<table>
  <caption>Webhook 通知の詳細</caption>
  <tr>
     <th>フィールド</th>
     <th>説明</th>
  </tr>
  <tr>
    <td>名前</td>
    <td>通知の固有 ID。このフィールドは必須です。</td>
  </tr>
  <tr>
    <td>タイプ </td>
    <td>**「Webhook」**を選択します。</td>
  </tr>
  <tr>
    <td>Webhook URL (Webhook URL)</td>
    <td>POST を行う URL を入力します。</td>
  </tr>
  <tr>
  <td>証明書の検証 (Verify certificates)</td>
    <td>証明書を検証する場合に選択します。</td>
  </tr>
  <tr>
    <td>Webhook ヘッダー (Webhook headers)</td>
    <td>任意のヘッダーを入力します。</td>
  </tr>
  <tr>
    <td>Webhook 照会パラメーター (Webhook query parameters)</td>
    <td>任意の照会パラメーターを入力します。</td>
  </tr>
</table>

<table>
  <caption>Pager Duty 通知の詳細</caption>
  <tr>
     <th>フィールド</th>
     <th>説明</th>
  </tr>
  <tr>
    <td>名前</td>
    <td>通知の固有 ID。このフィールドは必須です。</td>
  </tr>
  <tr>
    <td>タイプ </td>
    <td>**「Pager Duty」**を選択します。</td>
  </tr>
  <tr>
    <td>API キー</td>
    <td>Pager Duty 通知の APIKey を入力します。</td>
  </tr>
</table>


5. **「OK」**をクリックして、指定した設定で新しい通知を作成します。

## 通知の編集
 1. ベータ版に参加した後、**「デバイス」-> 「モニタリング」**を選択します。 
 2. **「通知」**タブをクリックします。
3. **「アクション」->「通知の編集 (Edit Notification)」**をクリックします。
4. 通知の詳細を編集します。
5. **「OK」** をクリックして変更を受け入れます。

## 通知の削除
1. ベータ版に参加した後、**「デバイス」-> 「モニタリング」**を選択します。 
2. **「通知」**タブをクリックします。
3. **「アクション」->「通知の削除 (Delete Notification)」**をクリックします。
4. **「削除」**をクリックして、選択を確認します。

## デバイスへの複数の通知の追加
1. **「インフラストラクチャー」->「デバイス・リスト」->*「デバイス名」***を選択して、デバイスの詳細情報にアクセスします。
2. **「アクション」->「通知の管理 (Manage notifications)」**をクリックします。
4. クリックして、デバイスの通知の割り当て/解除を行います。

