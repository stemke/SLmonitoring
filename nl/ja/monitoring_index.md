---



copyright:
  years: 2014, 2017
lastupdated: "2017-11-01"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# モニタリング
{{site.data.keyword.BluSoftlayer_full}} は、デバイスの問題を必ず認識できるように、標準モニタリング・サービスと Nimsoft Monitoring の両方を提供しています。標準モニタリング・サービスには、Ping や IPMI 統計などの機能があります。Nimsoft Monitoring は、基本モニタリング、拡張モニタリング、プレミアム・モニタリングの 3 つのレベルのモニタリングで構成されています。標準モニタリングと Nimsoft Monitoring の両方のオファリングに含まれている各サービスにはさまざまな利点があり、ビジネス・ニーズに合うようにさまざまな料金オプションが用意されています。詳しくは、[{{site.data.keyword.cloud}} infrastructure monitoring & reporting](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window} を参照してください。

デバイスのモニタリングにより、ユーザーは Service Ping および Slow Ping を開始して、デバイスがオンラインであり、応答していることを確認できます。

割り当てられた時間枠 (Service Ping の場合は 1 秒、Slow Ping の場合は 5 秒) 内にエコーを受信しなかった場合、アカウントの E メール・アドレスにアラートが送信されます。**「状況」**フィールドの**「アップ」**の状況は、エコーを受信したことを示します。一方、**「ダウン」**は、エコーを受信しなかったことを示します。 

構成したモニターを表示するには、以下の手順を実行します。

1\. デバイス・リストから**「デバイス名」**をクリックして、デバイスにアクセスします。

2\. **「モニタリング」**タブをクリックします。現在のすべての ping がランディング・ページに表示されます (**「モニタリング」**タブは、少なくとも 1 つのモニターが構成されている場合にのみ表示されます)。



