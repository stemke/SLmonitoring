---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# 開始使用 IBM Cloud Monitoring（測試版）
{: #gettingstartedbeta}

此測試版監視應用程式建置在「{{site.data.keyword.BluSoftlayer_full}} 監視服務」上，可用於虛擬及裸機伺服器。如需開發此「測試版」程式的相關更新項目，請參閱 [IBM Cloud 部落格 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}。{:shortdesc}

## 必要條件

若要參與此「測試版」程式，您必須符合下列需求。
1. 您的 SoftLayer 帳戶必須使用 IBM ID 鑑別鏈結至 IBM Cloud 帳戶。若要鏈結帳戶，SoftLayer 帳戶上的「主要使用者」必須登入 [{{site.data.keyword.slportal}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com){: new_window}，並從**帳戶**功能表中，按一下**鏈結 Bluemix 帳戶！**。
2. 每一個要檢視「測試版」的使用者都必須鏈結至 IBM ID。如需相關資訊，請參閱[鏈結 IBM ID 使用者帳戶](/docs/account?topic=account-unifyingaccounts#link_customer_accounts)。
3. 每一個要檢視「測試版」的使用者都必須能夠存取「IBM Cloud 監視服務」。
   1. 從 [IBM Cloud 主控台 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://console.bluemix.net){: new_window}，選取**管理 -> 帳戶 -> 使用者**。
   2. 邀請使用者加入帳戶，或從清單中選取使用者。
   3. 選取**指派對資源的存取權**給使用者。
   4. 從**服務**中，選取 **IBM Cloud 監視服務**。
   5. 選取要授與所有區域之使用者的**角色**。

如果不符合這些必要條件，此時您無法存取「測試版」監視。


## 加入測試版

請遵循下列步驟，以開始監視「測試版」程式。加入「測試版」可啟用您帳戶中所有合格虛擬及裸機伺服器的服務。按一下結合不會影響現有的 Nimsoft 監視或資料。
1. （僅限裸機）[在裸機伺服器上安裝監視代理程式](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-)。
<table>
   <CAPTION>表 1. 選擇登入位置</CAPTION>
   <THEAD>
   <TR>
   <th>如果想要透過下列項目加入...</th>
   <th>則...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>IBM Cloud 型錄</td>
   <td>
   <ol>
   <li>開啟新的瀏覽器視窗，然後輸入 <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>。</li>
   <li>按一下<b>登入</b>鏈結。</li>
   <li>輸入電子郵件或 IBM ID，然後按一下<b>繼續</b>。</li>
   <li>輸入「密碼」，然後按一下<b>登入</b>。</li>
   <li>選取**基礎架構->裝置清單->*裝置名稱***，以存取裝置詳細資料。</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>客戶入口網站</td>
   <td>
   <ol>
   <li>開啟新的瀏覽器視窗，然後輸入 <a href="https://control.softlayer.com">https://control.softlayer.com</a>。</li>
   <li>輸入使用者名稱及「密碼」，然後按一下<b>登入</b>。或者，按一下<b>使用 IBM ID 登入</b>。然後，輸入電子郵件或 IBM ID，並按一下<b>繼續</b>。輸入密碼，然後按一下<b>登入</b>。即會開啟 {{site.data.keyword.slportal}} 的主頁面。</li>
     <li>從**裝置**中，按一下**裝置名稱**，以存取裝置詳細資料。</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. 選取**裝置 -> 監視**。按一下**加入測試版**，以檢視系統原則及通知測試版標籤。

## 後續步驟
1. 檢閱所收集之[度量值](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-)的詳細資料。
2. [建立或管理](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-)監視器通知。
3. [建立或管理](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-)系統原則。
4. [檢視警示](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-)。
5. 檢閱所選取裝置目前可用的「測試版」監視圖形資料。

|              度量值                                         |  說明                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU 使用率|   檢視每一個核心的 CPU 使用率百分比，以及跨核心的平均值。按一下索引鍵中的每一個度量值，以開啟或關閉圖形上的資料。
|公用網路|   檢視公用網路的入埠及出埠資料。按一下索引鍵中的每一個度量值，以開啟或關閉圖形上的資料。|
|專用網路|   檢視專用網路的入埠及出埠資料。按一下索引鍵中的每一個度量值，以開啟或關閉圖形上的資料。|
|記憶體使用率      | 檢視伺服器的記憶體使用率百分比    |
|磁碟用量    | 檢視從磁碟讀取或寫入磁碟的平均資料數量（以位元組為單位）或磁碟延遲。按一下索引鍵中的每一個度量值，以開啟或關閉圖形上的資料。|
|溫度                                                 |檢視裸機裝置的溫度（以度（攝氏）表示）。此資料不適用於所有裝置。
{: caption="表 1. 測試版度量值" caption-side="top"}   

## 限制
如果刪除裝置，不會刪除相關聯的監視原則。請注意，您必須手動刪除這些原則的裝置。

度量值資料只能使用 15 天。

一次只能存在 10 個監視原則。不過，一個原則可以套用至多個裝置。

## 疑難排解
若要檢視部分度量值，例如記憶體使用率，伺服器上需要 Xen 工具。如需安裝 Xen 工具的相關資訊，請參閱[準備及匯入映像檔](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images)。

## 意見
若要對此「測試版」提供意見，請選取**裝置 -> 監視**或裝置詳細資料頁面，然後按一下**留下意見**以完成簡短的意見調查。若要離開「測試版」並回到標準視圖，請按一下**裝置 -> 監視**頁面底端的**離開測試版**鏈結。
