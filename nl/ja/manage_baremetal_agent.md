---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# IBM Cloud Monitoring Service for IaaS Bare Metal Agent の管理 (ベータ)

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent は、自身がインストールされたデバイスからメトリック・データを収集し、メトリック・ストレージに送信します。メトリック・ストレージのデータを、ユーザー・インターフェースで使用して単純なモニタリングを行えます。Grafana で使用すると、高度な照会を実行できます。
IBM Cloud Monitoring Service for IaaS Bare Metal Agent を使用する場合は、次の手順に従って、サーバーでサービスを表示、停止、開始、アンインストールできます。
{:shortdesc}

<table>
   <CAPTION>表 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>実行する操作</th>
   <th>Linux の場合</th>
     <th>FreeBSD の場合</th>
     <th>Windows の場合</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>サービスの状況の表示</td>
   <td>
   コマンド `service monitoring status` を使用します
   </td>
     <td>
   コマンド `service monitoring status` を使用します
   </td>
     <td>
   コマンド `sc.exe query monitoring` を使用します
   </td>
   </tr>
   <tr>
   <td>モニタリング・サービスの停止</td>
   <td>
   コマンド `service monitoring stop` を使用します
   </td>
     <td>
   コマンド `service monitoring stop` を使用します
   </td>
     <td>
   コマンド `sc.exe stop monitoring` を使用します
   </td>
   </tr>
       <tr>
   <td>モニタリング・サービスの開始</td>
   <td>
   コマンド `service monitoring start` を使用します
   </td>
     <td>
   コマンド `service monitoring start` を使用します
   </td>
     <td>
   コマンド `sc.exe start monitoring` を使用します
   </td>
   </tr>
       <tr>
   <td>モニタリング・サービスのアンインストール</td>
   <td>以下のコマンドを入力します。
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>以下のコマンドを入力します。
  <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>以下の手順を実行します。
 <ol>
       <li>**「プログラムの追加と削除」**を開きます。</li>
       <li>**「IBM Cloud Monitoring Agent」**を選択します。</li>
   <li>**「アンインストール」**をクリックします。</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>
