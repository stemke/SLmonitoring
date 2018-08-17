---
copyright:
  years: 2018
lastupdated: "2018-05-18"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Überwachungsbenachrichtigungen erstellen und verwalten (Beta)
Eine Benachrichtigung beschreibt die verwendete Methode und die entsprechenden Details beim Auslösen eines Alerts. Um beispielsweise eine Warn- oder Fehlerbenachrichtigung für eine Metrik zu erhalten, definieren Sie jeweils eine Regel, die den Warnungsschwellenwert und den Fehlerschwellenwert überwacht.
{:shortdesc} 

## Benachrichtigung erstellen
 
 1. Wenn Sie erfolgreich an der Betaversion teilnehmen, wählen Sie **Geräte -> Überwachung** aus. 
 2. Klicken Sie auf die Registerkarte **Benachrichtigungen**.
 3. Klicken Sie auf **Benachrichtigung erstellen**.
 4. Geben Sie die Informationen für die neue Benachrichtigung ein. 

<table>
  <caption>Details einer E-Mail-Benachrichtigung</caption>
  <tr>
     <th>Feld</th>
     <th>Beschreibung</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Eine eindeutige ID der Benachrichtigung. Dieses Feld ist erforderlich.</td>
  </tr>
  <tr>
    <td>Typ</td>
    <td>Wählen Sie **E-Mail** aus.</td>
  </tr>
  <tr>
    <td>E-Mail-Adresse</td>
    <td>Geben Sie die E-Mail-Adresse des Empfängers ein.</td>
  </tr>
</table>

<table>
  <caption>Details einer Webhook-Benachrichtigung</caption>
  <tr>
     <th>Feld</th>
     <th>Beschreibung</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Eine eindeutige ID der Benachrichtigung. Dieses Feld ist erforderlich.</td>
  </tr>
  <tr>
    <td>Typ</td>
    <td>Wählen Sie **Webhook** aus.</td>
  </tr>
  <tr>
    <td>Webhook-URL</td>
    <td>Geben Sie die URL ein, an der die POST-Anforderung durchgeführt werden soll.</td>
  </tr>
  <tr>
  <td>Zertifikate überprüfen</td>
    <td>Wählen Sie diese Option zum Überprüfen von Zertifikaten aus.</td>
  </tr>
  <tr>
    <td>Webhook-Header</td>
    <td>Geben Sie beliebige Header ein.</td>
  </tr>
  <tr>
    <td>Webhook-Abfrageparameter</td>
    <td>Geben Sie beliebige Abfrageparameter ein.</td>
  </tr>
</table>

<table>
  <caption>Details einer PagerDuty-Benachrichtigung</caption>
  <tr>
     <th>Feld</th>
     <th>Beschreibung</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Eine eindeutige ID der Benachrichtigung. Dieses Feld ist erforderlich.</td>
  </tr>
  <tr>
    <td>Typ</td>
    <td>Wählen Sie **PagerDuty** aus.</td>
  </tr>
  <tr>
    <td>API-Schlüssel</td>
    <td>Geben Sie den API-Schlüssel für PagerDuty-Benachrichtigungen ein.</td>
  </tr>
</table>


5. Klicken Sie auf **OK**, um die neuen Benachrichtigungen mit den von Ihnen angegebenen Einstellungen zu erstellen.

## Benachrichtigung bearbeiten
 1. Wenn Sie erfolgreich an der Betaversion teilnehmen, wählen Sie **Geräte -> Überwachung** aus. 
 2. Klicken Sie auf die Registerkarte **Benachrichtigungen**.
3. Klicken Sie auf **Aktionen->Benachrichtigung bearbeiten**.
4. Bearbeiten Sie die Benachrichtigungsdetails.
5. Klicken Sie auf **OK**, um die Änderungen zu übernehmen.

## Benachrichtigung löschen
1. Wenn Sie erfolgreich an der Betaversion teilnehmen, wählen Sie **Geräte -> Überwachung** aus. 
2. Klicken Sie auf die Registerkarte **Benachrichtigungen**.
3. Klicken Sie auf **Aktionen->Benachrichtigung löschen**.
4. Klicken Sie auf **Löschen**, um Ihre Auswahl zu bestätigen.

## Mehrere Benachrichtigungen zu einem Gerät hinzufügen
1. Wählen Sie **Infrastruktur->Geräteliste->*Gerätename*** aus, um auf die Gerätedetails zuzugreifen.
2. Klicken Sie auf **Aktionen->Benachrichtigungen verwalten**.
4. Klicken Sie entsprechend, um Benachrichtigungen für das Gerät zuzuweisen oder zu entfernen.

