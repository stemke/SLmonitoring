---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# IBM Cloud Monitoring 入門 (ベータ)
{: #gettingstartedbeta}

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service に基づいて構築されたこのベータ版のモニタリング・アプリケーションは、仮想サーバーおよびベア・メタル・サーバーで使用できます。 このベータ・プログラムの開発に関する最新情報については、[IBM Cloud Blog ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window} を参照してください。
{:shortdesc}

## 前提条件

このベータ・プログラムに参加するには、以下の要件を満たす必要があります。
1. SoftLayer アカウントを IBM ID 認証を使用して IBM Cloud アカウントにリンクする必要があります。アカウントをリンクするには、SoftLayer アカウントのマスター・ユーザーが [{{site.data.keyword.slportal}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com){: new_window} にログインし、**「アカウント」**メニューで**「Bluemix アカウントをリンクします」**をクリックします。
2. ベータ版を表示するすべてのユーザーは、IBM ID にリンクされている必要があります。 詳しくは、[IBM ID ユーザー・アカウントのリンク](/docs/account?topic=account-unifyingaccounts#link_customer_accounts)を参照してください。
3. ベータ版を表示するすべてのユーザーは、IBM Cloud Monitoring Service に対するアクセス権限を持っていなければなりません。
   1. [IBM Cloud コンソール ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://console.bluemix.net){: new_window} で、**「管理」->「アカウント」->「ユーザー」**を選択します。
   2. アカウントにユーザーを招待するか、リストからユーザーを選択します。
   3. ユーザーに対して**「リソースへのアクセス権限の割り当て」**を選択します。
   4. **「サービス」**から、**「IBM Cloud Monitoring Service」**を選択します。
   5. すべての地域でそのユーザーに付与する**役割**を選択します。

これらの前提条件を満たしていない場合は、現時点ではベータ・モニタリングにアクセスできません。


## ベータ版への参加

モニタリング・ベータ・プログラムの使用を開始するには、以下の手順に従います。 ベータ版に参加すると、アカウント内の適用対象のすべての仮想サーバーとベア・メタル・サーバーに対してサービスが有効になります。 「参加 (join)」をクリックしても、既存の Nimsoft モニタリングやデータには影響しません。
1. (ベア・メタルのみ) [ベア・メタル・サーバーにモニタリング・エージェントをインストールします](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-)。
<table>
   <CAPTION>表 1. ログイン場所の選択</CAPTION>
   <THEAD>
   <TR>
   <th>参加するために使用する方法</th>
   <th>手順</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>IBM Cloud カタログ</td>
   <td>
   <ol>
   <li>新しいブラウザー・ウィンドウを開き、<a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a> と入力します。</li>
   <li><b>「ログイン」</b>リンクをクリックします。 </li>
   <li>E メールまたは IBM ID を入力し、<b>「続行」</b>をクリックします。</li>
   <li>パスワードを入力し、<b>「ログイン」</b>をクリックします。</li>
   <li>**「インフラストラクチャー」->「デバイス・リスト」->*「デバイス名」***を選択して、デバイスの詳細情報にアクセスします。</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>カスタマー・ポータル</td>
   <td>
   <ol>
   <li>新しいブラウザー・ウィンドウを開き、<a href="https://control.softlayer.com">https://control.softlayer.com</a> と入力します。</li>
   <li>ユーザー名とパスワードを入力し、<b>「ログイン」</b> をクリックします。 あるいは、<b>「IBM ID でログイン」</b>をクリックします。 次に、E メールまたは IBM ID を入力し、<b>「続行」</b>をクリックします。 パスワードを入力し、<b>「ログイン」</b>をクリックします。 {{site.data.keyword.slportal}}のメインページが開きます。</li>
     <li>**「デバイス」**から**「デバイス名」**をクリックして、デバイスの詳細にアクセスします。</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. **「デバイス」->「モニタリング」**を選択します。 **「ベータに参加 (Join the beta)」**をクリックして、システム・ポリシーと通知のベータ・タブを表示します。

## 次の手順
1. 収集された[メトリック](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-)の詳細を確認します。
2. モニター通知を[作成または管理](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-)します。
3. システム・ポリシーを[作成または管理](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-)します。
4. [アラートを表示](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-)します。
5. 選択したデバイスについての現在使用できるベータ・モニタリング・グラフ・データを確認します。

|              メトリック                                      |  説明                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU 使用率                                                 |   各コアの CPU 使用率 (%) とすべてのコアの平均を表示します。 キーの各メトリックをクリックして、グラフでのデータの表示/非表示を切り替えられます。
|パブリック・ネットワーク                                   |   パブリック・ネットワークのインバウンド・データおよびアウトバウンド・データを表示します。 キーの各メトリックをクリックして、グラフでのデータの表示/非表示を切り替えられます。       |
|プライベート・ネットワーク                                 |   プライベート・ネットワークのインバウンド・データおよびアウトバウンド・データを表示します。 キーの各メトリックをクリックして、グラフでのデータの表示/非表示を切り替えられます。           |
|メモリー使用率    | サーバーのメモリー使用率 (%) を表示します     |
|ディスク使用状況    | ディスクとの間で読み書きされている平均データ量をバイト数で表示します。またはディスク待ち時間を表示します。 キーの各メトリックをクリックして、グラフでのデータの表示/非表示を切り替えられます。    |
|温度                                                 |ベア・メタル・デバイスの温度を摂氏度で表示します。 このデータは、すべてのデバイスで使用できるわけではありません。
{: caption="表 1. ベータ・メトリック" caption-side="top"}   

## 制限
デバイスを削除しても、関連するモニター・ポリシーは削除されません。 これらのポリシーのデバイスは手動で削除する必要があることに注意してください。

メトリック・データを使用できるのは 15 日間のみです。

同時に存在できるモニタリング・ポリシーは 10 個のみです。 ただし、1 つのポリシーを複数のデバイスに適用できます。

## トラブルシューティング
メモリー使用率などの一部のメトリックを表示するには、サーバーに Xen ツールが必要です。Xen ツールのインストール方法については、[イメージの準備およびインポート](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images)を参照してください。

## フィードバック
このベータ版に関するフィードバックを提供するには、**「デバイス」->「モニタリング」**またはデバイスの詳細ページを選択し、**「フィードバックを送信 (Leave feedback)」**をクリックし、簡単なアンケートに答えてください。 ベータ版を終了して標準ビューに戻るには、**「デバイス」->「モニタリング」**ページの下部にある**「ベータ版の終了 (Leave the Beta)」**リンクをクリックします。
