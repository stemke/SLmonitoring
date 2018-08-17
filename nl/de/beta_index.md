---
copyright:
  years: 2017, 2018
lastupdated: "2018-05-16"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# Einführung in IBM Cloud Monitoring (Beta)

{: #gettingstartedbeta}
Diese Beta-Überwachungsanwendung, die auf dem {{site.data.keyword.BluSoftlayer_full}} Monitoring-Service basiert, steht für virtuelle Server und Bare-Metal-Server zur Verfügung. Aktualisierungen zur Entwicklung dieses Betaprogramms finden Sie im [Blog zu IBM Cloud ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}.

{:shortdesc}

## Voraussetzungen

Um dieses Betaprogramm nutzen zu können, müssen die folgenden Voraussetzungen erfüllt sein.
1. Ihr SoftLayer-Konto muss mit einem IBM Bluemix-Konto verbunden sein. Zum Verbinden eines Kontos muss sich der Masterbenutzer des SoftLayer-Kontos beim [{{site.data.keyword.slportal_full}}](https://control.softlayer.com) anmelden und im Menü **Konto** auf die Option zum **Verknüpfen eines Bluemix-Kontos** klicken.
2. Benutzer, die die Betaversion anzeigen möchten, müssen mit einer IBM ID verknüpft sein. Weitere Informationen finden Sie in der Veröffentlichung zum [Verknüpfen von IBMid Benutzerkonten](../../account/softlayerlink.html#link_customer_accounts).
3. Benutzer, die die Betaversion anzeigen möchten, müssen Zugriff auf den IBM Cloud Monitoring-Service haben. 
   1. Wählen Sie in der [BlueMix-Konsole](https://console.bluemix.net) die Option **Verwalten -> Konto -> Benutzer** aus.
   2. Laden Sie den Benutzer für das Konto ein oder wählen Sie den Benutzer aus der Liste aus.
   3. Wählen Sie **Zugriff auf Ressourcen zuweisen** für den Benutzer aus.
   4. Wählen Sie unter **Service** den Eintrag **IBM Cloud Monitoring Service** aus. 
   5. Wählen Sie die **Rolle** aus, die dem Benutzer für alle Regionen erteilt werden soll.

Wenn Sie diese Voraussetzungen nicht erfüllen, können Sie zu diesem Zeitpunkt nicht auf die Beta-Überwachungsanwendung zugreifen.


## Am Betaprogramm teilnehmen 

Führen Sie die nachfolgenden Schritte als Einführung in das Beta-Überwachungsprogramm aus. Durch die Teilnahme am Betaprogramm wird der Service für alle infrage kommenden virtuellen Server und Bare-Metal-Server in Ihrem Konto aktiviert. Die Auswahl der Option zum Teilnehmen hat keinerlei Auswirkungen auf die Nimsoft-Überwachung oder die entsprechenden Daten.
1. (Nur Bare-Metal) [Installieren Sie den Überwachungsagent auf dem Bare-Metal-Server](install_observer.html). 
<table>
   <CAPTION>Tabelle 1. Protokoll an Position auswählen</CAPTION>
   <THEAD>
   <TR>
   <th>Gewünschte Teilnahme an...</th>
   <th>Aktion...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>IBM Cloud-Katalog</td>
   <td>
   <ol>
   <li>Öffnen Sie ein neues Browserfenster und geben Sie <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a> ein.</li>
   <li>Klicken Sie auf den Link <b>Anmeldung</b>. </li>
   <li>Geben Sie Ihre E-Mail oder IBMid ein und klicken Sie auf <b>Weiter</b>.</li>
   <li>Geben Sie Ihr Kennwort ein und klicken Sie auf <b>Anmelden</b>.</li>
   <li>Wählen Sie **Infrastruktur->Geräteliste->*Gerätename*** aus, um auf die Gerätedetails zuzugreifen.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Kundenportal</td>
   <td>
   <ol>
   <li>Öffnen Sie ein neues Browserfenster und geben Sie <a href="https://control.softlayer.com">https://control.softlayer.com</a> ein.</li>
   <li>Geben Sie Ihren Benutzernamen und das Kennwort ein und klicken Sie auf <b>Anmeldung</b>. Alternativ können Sie auf <b>Melden Sie sich mit der IBMid an</b> klicken. Geben Sie dann Ihre E-Mail oder IBMid ein und klicken Sie auf <b>Weiter</b>. Geben Sie Ihr Kennwort ein und klicken Sie auf <b>Anmeldung</b>. Die Hauptseite des {{site.data.keyword.slportal}}s wird geöffnet.</li>
     <li>Klicken Sie unter **Geräte** auf den **Gerätenamen**, um auf die Gerätedetails zuzugreifen.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. Wählen Sie **Geräte -> Überwachung** aus. Klicken Sie auf **An Beta teilnehmen**, um die Registerkarten mit den Systemrichtlinien und Benachrichtigungen des Betaprogramms anzuzeigen.

## Nächste Schritte
1. Überprüfen Sie die Details der erfassten [Metriken](metrics.html).
2. [Erstellen oder verwalten](create_notification.html) Sie eine Überwachungsbenachrichtigung.
3. [Erstellen oder verwalten](create_policy.html) Sie eine Systemrichtlinie.
4. [Zeigen Sie Alerts an](view_alerts.html).
5. Überprüfen Sie die aktuell verfügbaren Diagrammdaten der Beta-Überwachung für ein ausgewähltes Gerät.

|              Metriken                                     |  Beschreibung                                       |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU-Auslastung                                             |   Zeigen Sie die CPU-Auslastung in % für jeden Kern und einen Durchschnitt über Kerne hinweg an. Klicken Sie auf die einzelnen Metriken im Schlüssel, um die Daten im Diagramm ein- oder auszublenden.
|Öffentliches Netz                                          |   Zeigen Sie eingehende und abgehende Daten für das öffentliche Netz an. Klicken Sie auf die einzelnen Metriken im Schlüssel, um die Daten im Diagramm ein- oder auszublenden.       |
|Privates Netz                                              |   Zeigen Sie eingehende und abgehende Daten für das private Netz an. Klicken Sie auf die einzelnen Metriken im Schlüssel, um die Daten im Diagramm ein- oder auszublenden.           |
|Speicherauslastung    | Zeigen Sie die Speicherauslastung in % für den Server an.     |
|Plattenbelegung       | Zeigen Sie das durchschnittliche Datenvolumen, das auf die Platte oder von der Platte gelesen oder geschrieben wird, in Byte oder die Plattenlatenz an. Klicken Sie auf die einzelnen Metriken im Schlüssel, um die Daten im Diagramm ein- oder auszublenden.    |
|Temperatur                                                  |Zeigen Sie die Temperatur des Bare-Metal-Geräts in Grad Celsius an. Diese Daten sind nicht für alle Geräte verfügbar.
{: caption="Tabelle 1. Beta-Metriken" caption-side="top"}   

## Einschränkungen 
Wenn ein Gerät gelöscht wird, werden die zugehörigen Überwachungsrichtlinien nicht gelöscht. Beachten Sie, dass Sie das Gerät für diese Richtlinien manuell löschen müssen.

Metrikendaten sind nur für 15 Tage verfügbar.

Es können nur 10 Überwachungsrichtlinien gleichzeitig vorhanden sein. Eine Richtlinie kann jedoch auf mehrere Geräte angewendet werden.

## Fehlerbehebung
Zum Anzeigen einiger Metriken, wie Speicherauslastung, müssen Xen-Tools auf dem Server vorhanden sein. Informationen zum Installieren von Xen-Tools finden Sie in [Images vorbereiten und installieren](../image-templates/import-image.html#preparing-and-importing-images).

## Feedback 
Um Feedback zu dieser Betaversion zu geben, wählen Sie **Geräte -> Überwachung** oder die Seite mit den Gerätedetails aus und klicken Sie auf **Feedback geben**, um an einer kurzen Befragung teilzunehmen. Um die Betaversion zu verlassen und zurück zur Standardansicht zu wechseln, klicken Sie auf der Seite **Geräte -> Überwachung** auf den Link **Beta verlassen**.


