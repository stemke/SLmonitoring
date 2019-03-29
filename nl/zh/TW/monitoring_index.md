---

copyright:
  years: 2014, 2018
lastupdated: "2018-11-15"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 監視
{: #monitoring}

{{site.data.keyword.BluSoftlayer_full}} 同時提供「標準監視服務」及「Nimsoft 監視」，以確保您隨時都知道任何裝置問題。「標準監視服務」包括「連線測試」及「IPMI 統計資料」之類的特性。「Nimsoft 監視」由三個監視層次組成，包括基本、進階及高階監視。同時具有「標準監視」及「Nimsoft 監視」供應項目的每一個服務，提供各種權益，且有各種定價選項可供選擇，以符合您的商業需要。如需相關資訊，請參閱 [{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}。

監視裝置可讓使用者起始服務及慢速連線測試，以確保裝置處於線上且可回應。

如果在分配的時間範圍（服務 Ping 為 1 秒，慢速 Ping 為 5 秒）內收不到回應，則會將警示傳送至帳戶的電子郵件位址。**狀態**欄位中的**開啟**狀態指出已收到回應，而**關閉**則指出未收到回應。

若要檢視已配置的監視器，請遵循下列步驟：

1. 從「裝置清單」中，按一下**裝置名稱**以存取裝置。

2. 按一下**監視**標籤。在登陸頁面上，可以檢視所有現行 Ping（只有在配置了至少一個監視器時，才能看到**監視**標籤）。
