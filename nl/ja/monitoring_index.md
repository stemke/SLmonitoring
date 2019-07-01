---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 入門チュートリアル
{: #monitoring}

{{site.data.keyword.cloud}} は、デバイスの問題を必ず認識できるように、標準モニタリング・サービスと Nimsoft Monitoring の両方を提供しています。標準モニタリング・サービスには、Ping や IPMI 統計などの機能があります。Nimsoft Monitoring は、基本モニタリング、拡張モニタリング、プレミアム・モニタリングの 3 つのレベルのモニタリングで構成されています。 標準モニタリングと Nimsoft Monitoring の両方のオファリングに含まれている各サービスにはさまざまな利点があり、ビジネス・ニーズに合うようにさまざまな料金オプションが用意されています。詳しくは、[{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window} を参照してください。
{:shortdesc}

デバイスのモニタリングにより、Service Ping および Slow Ping を開始して、デバイスがオンラインであり、応答していることを確認できます。

割り当てられた時間フレーム (Service Ping の場合は 1 秒、Slow Ping の場合は 5 秒) 内にエコーを受信しなかった場合、アカウントの E メール・アドレスにアラートが送信されます。**「状況」**フィールドの**「アップ」**の状況は、エコーを受信したことを示します。一方、**「ダウン」**は、エコーを受信しなかったことを示します。

構成したモニターを表示するには、以下の手順を実行します。

1. コンソールのデバイス・メニューに移動します。詳しくは、[デバイスへのナビゲート](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)を参照してください。
2. **「デバイス」**メニューから**「デバイス・リスト」**を選択し、デバイスを選びます。
3. **「モニタリング」**タブをクリックします。 現在のすべての ping がランディング・ページに表示されます。 

**「モニタリング」**タブは、少なくとも 1 つのモニターが構成されている場合にのみ可視になります。
{:note}

