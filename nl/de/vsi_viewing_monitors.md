---

copyright:
  years: 2017
lastupdated: "2017-09-28"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Überwachungen anzeigen und verwalten
{: viewing-and-managing-monitors}

Durch die Überwachung eines Geräts können Benutzer Service-Pings und langsame Pings initiieren, um sicherzustellen, dass das Gerät online und betriebsbereit ist.
{:shortdesc}

Wenn im zugewiesenen Zeitrahmen (eine Sekunde für Service-Pings, fünf Sekunden für langsame Pings) kein Echo empfangen wird, wird ein Alert an die E-Mail-Adresse
im Konto gesendet. Ein aktiver Status **** im Feld **Status** zeigt an, dass ein Echo empfangen wurde, während ein inaktiver Status ****
angibt, dass kein Echo empfangen wurde. Wenn Sie eine einfache Überwachung konfiguriert haben, führen Sie die folgenden Schritte durch, um die Überwachung für ein Gerät anzuzeigen und zu verwalten.

   <table>
   <CAPTION>Tabelle 1. Geräteüberwachung anzeigen und verwalten</CAPTION>
   <THEAD>
   <TR>
   <th>Gewünschte Aktion...</th>
   <th>Vorgehensweise...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Überwachungen anzeigen</td>
   <td>
   <ol>
   <li>Klicken Sie in der Geräteliste auf den <b>Gerätenamen</b>, um auf das Gerät zuzugreifen.</li>
   <li>Klicken Sie auf die Registerkarte <b>Überwachung</b>. Alle aktuellen Pings können auf der Landing-Page angezeigt werden. (Die Registerkarte <b>Überwachung</b> ist nur sichtbar, wenn mindestens eine Überwachung konfiguriert ist.)</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Überwachung hinzufügen</td>
   <td>
   <ol>
   <li>Klicken Sie auf der Registerkarte <b>Überwachung</b> der Seite mit den Gerätedetails rechts auf der Seite auf <b>Überwachungen verwalten</b>, um mit diesem Gerät verknüpfte Überwachungen zu verwalten.</li>
   <li>Klicken Sie auf der Seite mit den Überwachungen auf die Registerkarte <b>Überwachung hinzufügen</b>.</li>
   <li>Wählen Sie die zu überwachende IP-Adresse aus der Liste <b>IP-Adresse</b> aus.</li>
   <li>Wählen Sie den Überwachungstyp aus der Liste <b>Überwachungstyp</b> aus.</li>
   <li>Richten Sie die Benachrichtigungsoptionen ein. Wählen Sie aus der Liste <b>Benachrichtigen?</b> die Option <b>Benutzer benachrichtigen</b> aus, um Benutzer über Probleme zu informieren, oder <b>Nichts tun</b>, um die Benutzerbenachrichtigung zu umgehen.</li>
   <li>Wählen Sie aus der Liste <b>Benachrichtigen Wartezeit</b> den Zeitrahmen für die Benutzerbenachrichtigung aus.</li>
   <li>Klicken Sie auf <b>Überwachung hinzufügen</b>, um die Überwachung für ein Gerät hinzuzufügen. Die neue Überwachung erscheint im Abschnitt zum <b>Bearbeiten vorhandener Überwachungen</b> in der Anzeige.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Vorhandene Überwachung bearbeiten</td>
   <td>
   <ol>
   <li>Klicken Sie auf der Seite für die Überwachungen unter der Überschrift <b>Vorhandene Überwachungen bearbeiten</b> auf ein beliebiges Überwachungsdetail, um die Überwachung für die Bearbeitung zu öffnen.</li>
   <li>Aktualisieren Sie eines der folgenden Felder: 'Überwachungstyp, 'Benachrichtigen', 'Benachrichtigen Wartezeit'.</li>
   <li>Klicken Sie auf <b>Aktualisieren</b>, um die Details zu aktualisieren. Klicken Sie auf <b>Abbrechen</b>, um die Bearbeitung abzubrechen.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Überwachung entfernen</td>
   <td>
   <ol>
   <li>Klicken Sie auf der Seite für die Überwachungen unter der Überschrift <b>Vorhandene Überwachungen bearbeiten</b> neben den Überwachungsdetails auf das Symbol zum Entfernen.</li>
   <li>Klicken Sie auf <b>Ja</b>, um die Überwachung zu entfernen. Klicken Sie auf <b>Nein</b>, um die Aktion abzubrechen.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
   </table>

## Nächste Schritte

- Wenn eine neue Überwachung hinzugefügt wird, wird die Überwachung auf der Registerkarte **Überwachung** angezeigt. Die Überwachung sendet jede fünf Minuten einen Ping an das Gerät und erwartet basierend auf dem ausgewählten Pingtyp eine entsprechende Antwort. Wird die erwartete Antwort nicht empfangen, wird im angegebenen Zeitrahmen eine E-Mail an die Benachrichtigungs-E-Mail-Adresse für das Konto gesendet, wenn die Benachrichtigungsoption ausgewählt ist.
- Wenn eine Überwachung bearbeitet wird, funktioniert die Überwachung weiterhin, wie in den Überwachungsdetails angegeben. Wenn der Typ geändert wird, ändert sich auch die Zeitdauer für den Empfang des erwarteten Pingsignals. Wenn die Benachrichtigungsoptionen geändert werden, ändert sich basierend auf der neuen Auswahl die Art und Weise, wie Benutzer über einen fehlgeschlagenen Versuch benachrichtigt werden. Die Überwachung bleibt über die Registerkarte **Überwachung** zugänglich.
- Wenn eine Überwachung entfernt wird, funktioniert die Überwachung für das Gerät nicht mehr. Alle Überwachungsvorgänge, die mit der entfernten Überwachung verknüpft sind, werden gestoppt und und die Überwachung wird nicht mehr auf der Registerkarte **Überwachung** angezeigt.
