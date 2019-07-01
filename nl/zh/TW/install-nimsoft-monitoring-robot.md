---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 安裝及管理 Nimsoft Monitoring Robot
{: #installing-and-managing-the-nimsoft-monitoring-robot}

若要容許進階監視在現有的 {{site.data.keyword.baremetal_short}} 或 {{site.data.keyword.BluVirtServers_short}} 上運作，請安裝 Nimsoft Monitoring Robot。Nimsoft Monitoring Robot 可讓監視管理系統與專用網路上的裸機伺服器或虛擬伺服器進行通訊。在安裝 Nimsoft Monitoring Robot 之後，它可能需要大約 5 - 10 分鐘，才能在 {{site.data.keyword.cloud}} 主控台上變成可用。請完成下列步驟，在 Windows 或 Linux 中安裝 Nimsoft Monitoring Robot。

## 必要條件

安裝之前，必須在專用網路上開啟下列埠：

* tcp/48000
* tcp/48001
* tcp/48002

此外，對專用網路開啟埠 tcp/48003 到 tcp/50000，以容許 API 所使用的完整功能。如果未開啟這些埠，則會影響部分監視代理程式。如果在配置期間發生錯誤，請先確定這些埠已開啟，再開立問題單以進行呈報。

* 某些監視代理程式（例如「Tomcat 監視代理程式」）需要 **openjdk**。
* 部分 64 位元 Linux 發行套件需要 **glibc.i686** 和 **nss-softtokn-freebl.i686**。
* **FreeBSD** 不支援監視系統。

如果由於 Nimsoft Robot 發生通訊錯誤而導致配置監視服務時發生錯誤，則配置處理程序可能由於連線功能有限而暫停。有限的連線功能通常是防火牆或其他安全軟體所造成的，而這些防火牆或安全軟體正在封鎖從 Nimsoft 管理伺服器存取系統。請遵循下列步驟來重新啟動監視服務的佈建：

## 重新啟動監視代理程式的佈建
{: #restarting-provisioning-of-a-monitoring-agent}

請完成下列步驟來重新啟動監視服務的佈建。
1. 導覽至主控台的裝置功能表。如需相關資訊，請參閱[導覽至裝置](https://test.cloud.ibm.com/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)。
2. 從**裝置**功能表，選取**監視**。
3. 找出正在為其配置監視的系統。
4. 選取**進階**區段中的**重新部署所有代理程式**。
5. 在**蹦現**頁面上選擇監視範本。
6. 按一下**重新部署**。

## 在 Windows 中安裝
{: #install-windows}

1. 造訪 http://downloads.service.softlayer.com/nimsoft/ 以將最新版的「Windows 安裝程式」下載至裝置，以進行安裝（您必須連接至客戶 VPN）。
2. 以「管理者」身分執行 Nimsoft Monitoring Robot 檔案。

## 在 Linux 中安裝
{: #install-linux}

1. 透過客戶 VPN 連接至專用網路。
2. 下載 [32 位元 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} 或 [64 位元 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} Linux 安裝程式至裝置上以便安裝。[Nimsoft 安裝程式 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://downloads.service.softlayer.com/nimsoft/){: new_window} 也提供 Debian 及 Ubuntu 版本。
3. 執行下列指令來完成安裝，如果您是執行 64 位元安裝，則將 32 取代為 64：

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## 後續步驟

在您執行安裝之後，系統會自動完成處理程序。在 Windows 中，會出現一則訊息，確認安裝成功或包含所發生之任何錯誤的相關資訊。

