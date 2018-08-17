---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Nimsoft Monitoring Robot のインストールおよび管理

既存の {{site.data.keyword.baremetal_short}} または {{site.data.keyword.BluVirtServers_short}} に対して拡張モニタリングが機能するようにするには、Nimsoft Monitoring Robot をインストールします。Nimsoft Monitoring Robot は、モニタリング管理システムがプライベート・ネットワーク上でベア・メタル・サーバーまたは仮想サーバーと通信できるようにします。Nimsoft Monitoring Robot をインストールした後、{{site.data.keyword.slportal_full}}で使用可能になるまでに約 5 分から 10 分かかります。Nimsoft Monitoring Robot を Windows または Linux にインストールするには、以下の手順に従います。

## 前提条件

インストールする前に、以下のポートをプライベート・ネットワーク上で開いておく必要があります。

* tcp/48000
* tcp/48001
* tcp/48002

さらに、プライベート・ネットワークでポート tcp/48003 から tcp/50000 を開き、API が使用するすべての機能を使用可能な状態にしてください。これらのポートを開かないと、一部のモニタリング・エージェントが影響を受けます。構成中にエラーが発生した場合は、エスカレーションのチケットを開く前に、これらのポートが開いていることを確認してください。 

* Tomcat モニタリング・エージェントなどの特定のモニタリング・エージェントには、**openjdk** が必要です。

* 一部の 64 ビット Linux ディストリビューションには、**glibc.i686** および **nss-softtokn-freebl.i686** が必要です。

* モニタリング・システムは **FreeBSD** ではサポートされません。
* モニタリング・システムは **Ubuntu 16** ではサポートされません。
* モニタリング・システムは **Windows 2016** ではサポートされません。

Nimsoft ロボットとの通信エラーのためにモニタリング・サービスの構成中にエラーが発生すると、接続が制限されるために構成プロセスが一時停止する可能性があります。接続が制限される理由は、多くの場合、Nimsoft 管理サーバーからシステムへのアクセスが、ファイアウォールまたはその他のセキュリティー・ソフトウェアによってブロックされているからです。次の手順に従って、モニタリング・サービスのプロビジョニングを再開してください。

## モニタリング・エージェントのプロビジョニングの再開

1. **「デバイス」**メニューに移動して、**「モニタリング」**を選択します。
* モニタリングを構成するシステムを見つけます。
* 右側の列の**「拡張」**ドロップダウンで**「すべてのエージェントの再デプロイ」**を選択します。
* **「ポップイン (Pop-In)」**ページでモニタリング・テンプレートを選択します。
* **「再デプロイ」**をクリックします。

## Windows へのインストール

1. http://downloads.service.softlayer.com/nimsoft を参照し、Windows インストーラーの最新バージョンをインストールするためにデバイスにダウンロードします (VPN に接続する必要があります)。
* Nimsoft Monitoring Robot ファイルを管理者として実行します。

## Linux へのインストール

1. VPN を介してプライベート・ネットワークに接続します。
* [32 ビット](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz) または [64 ビット](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz)の Linux インストーラーを、インストールするためにデバイスにダウンロードします。Debian バージョンと Ubuntu バージョンの [Nimsoft インストーラー](http://downloads.service.softlayer.com/nimsoft/)も用意されています。

* 次のコマンドを実行して、インストールを実行します。64 ビット・インストールを実行する場合は、32 を 64 に置き換えてください。


        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## 次の手順

インストールを実行すると、システムが自動的にプロセスを実行します。Windows では、正常にインストールされたことを確認するメッセージ、または発生したエラーに関する情報を示すメッセージが表示されます。
