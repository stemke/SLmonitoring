---
copyright:
  years: 2018
lastupdated: "2018-04-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# IBM Cloud Monitoring Service for IaaS Bare Metal Agent のインストール (ベータ)

既存の {{site.data.keyword.baremetal_short}} に対して拡張モニタリングが機能するようにするには、以下の手順に従って、{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent をベア・メタル・デバイスにインストールします。


## 前提条件
インストーラーをダウンロードして実行するために、ベア・メタル・デバイスに接続する必要があります。

## Windows へのインストール

1. Windows IBM Cloud Monitoring Agent インストーラーをダウンロードします。[ダウンロード](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi)
2. ターゲット・マシンでインストーラーを実行します。 

## Linux へのインストール

1. Linux IBM Cloud Monitoring Agent インストーラーをダウンロードします。[ダウンロード](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz)
2. ターゲット・マシンでインストーラーを unzip します。`tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. linux_install.sh スクリプトを実行します。

        
## FreeBSD へのインストール
1. FreeBSD IBM Cloud Monitoring Agent インストーラーをダウンロードします。[ダウンロード](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz)
2. ターゲット・マシンでインストーラーを unzip します。`tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. freebsd_install.sh スクリプトを実行します。 

## 次の手順

インストールを実行すると、システムが自動的にプロセスを実行します。Windows では、正常にインストールされたことを確認するメッセージ、または発生したエラーに関する情報を示すメッセージが表示されます。

ファイアウォールを使用している場合は、ファイアウォールを介してデータを渡すことを IBM Cloud Monitoring Agent に許可する必要があります。エージェントは、アウトバウンド HTTPS 通信にポート 8090 を使用します。許可する必要がある IP アドレスについて詳しくは、[ロード・バランサーの IP 範囲](https://console.bluemix.net/docs/infrastructure/hardware-firewall-dedicated/ips.html#load-balancer-ips)を参照してください。
