---

copyright:
  years: 2018
lastupdated: "2018-04-20"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 安裝 IBM Cloud Monitoring Service for IaaS Bare Metal Agent（測試版）

若要容許進階監視在現有的 {{site.data.keyword.baremetal_short}} 上運作，請遵循下列步驟，在裸機裝置上安裝 {{site.data.keyword.BluSoftlayer_full}} Monitoring Servicefor IaaS Bare Metal Agent。

## 必要條件
您必須連接至裸機裝置，才能下載並執行安裝程式。

## 在 Windows 中安裝

1. 下載 Windows IBM Cloud Monitoring Agent 安裝程式。[下載 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi){: new_window}
2. 在目標機器上執行安裝程式。

## 在 Linux 中安裝

1. 下載 Linux IBM Cloud Monitoring Agent 安裝程式。[下載 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz){: new_window}
2. 將它解壓縮到目標機器上。
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. 執行 linux_install.sh Script。


## 在 FreeBSD 中安裝
1. 下載 FreeBSD IBM Cloud Monitoring Agent 安裝程式。[下載 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz){: new_window}
2. 將它解壓縮到目標機器上。
       `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. 執行 freebsd_install.sh Script。

## 後續步驟

在您執行安裝之後，系統會自動完成處理程序。在 Windows 中，會出現一則訊息，確認安裝成功或包含所發生之任何錯誤的相關資訊。

如果使用防火牆，您可能需要容許 IBM Cloud Monitoring Agent 透過它來傳遞資料。代理程式使用埠 8090 進行出埠 HTTPS 通訊。如需您可能需要容許之 IP 位址的相關資訊，請參閱[負載平衡器 IP 範圍](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-load-balancer-ips#load-balancer-ips)。
