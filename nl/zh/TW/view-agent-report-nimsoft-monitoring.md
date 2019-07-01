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

# 檢視 Nimsoft 監視的代理程式報告
{: #viewing-an-agent-report-for-nimsoft-monitoring}

可在代理程式報告中取得「Nimsoft 監視」的監視詳細資料，其會提供代理程式配置方式的特定詳細資料。{:shortdesc}

## 開始之前
首先，請導覽至裝置功能表，並確定您有正確的帳戶許可權可以完成作業。

* 導覽至主控台的裝置功能表。如需相關資訊，請參閱[導覽至裝置](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)。
* 確定您有任何必要的帳戶許可權及裝置存取權。只有帳戶擁有者，或具有**管理使用者**標準基礎架構許可權的使用者，才能調整許可權。

如需許可權的相關資訊，請參閱[標準基礎架構許可權](/docs/iam?topic=iam-infrapermission#infrapermission)及[管理裝置存取權](/docs/vsi?topic=virtual-servers-managing-device-access)。

## 檢視 Nimsoft 監視的代理程式報告
{: #viewing-agent-report-nimsoft-monitoring-steps}

請完成下列步驟，以檢視 Nimsoft Monitoring 的代理程式報告。

1. 從**監視**頁面的**動作**功能表中，選取**檢視代理程式報告**。
2. 從**代理程式**清單中，選取要檢視的代理程式。

  可用的代理程式依裝置而有所不同，且相依於套用至裝置的監視套件。
  {:note}
  
3. 完成所有剩餘的區段，包括下列一個以上的動作：

  每一個代理程式都有所不同，且不包括每一個區段或度量值。此畫面上的可用選項視每一個代理程式可用的配置選項而定。
  {:note}
  
  * 從**區段**清單中，選取區段報告。
  * 從**檢視方式**清單中，選取報告的時段。
  * 在**選取要報告的度量值：**區段中，針對您要報告的每一個度量值按一下其勾選框。
    
    只有類似的度量值會出現在相同的圖形上。如果選擇了衝突的度量值，則會在要求圖形之後發生錯誤。
    {:note}
4. 按一下**繪製圖形**來繪製圖形。

## 後續步驟

在繪製代理程式報告的圖形之後，可以透過重複這些步驟，隨時重新繪製圖形來檢視不同的度量值。可在設定的時間量內產生的代理程式報告數目沒有限制。
