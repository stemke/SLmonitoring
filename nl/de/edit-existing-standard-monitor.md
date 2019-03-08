---

copyright:
  years: 2014, 2018
lastupdated: "2018-10-30"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Vorhandene Überwachung bearbeiten
Nachdem eine Überwachung zu einem Gerät hinzugefügt wurde, können Sie sie jederzeit ändern oder entfernen. Bei Änderungen an Überwachungen können der Typ und die Benachrichtigungsoptionen geändert werden, während beim Entfernen einer Überwachung die Überwachung vollständig abgebrochen wird. Führen Sie die folgenden Schritte durch, um eine vorhandene Überwachung zu bearbeiten.

1. Klicken Sie auf der Seite für die **Überwachungen** unter der Überschrift **Vorhandene Überwachungen bearbeiten** auf ein beliebiges Überwachungsdetail, um die Überwachung für die Bearbeitung zu öffnen.

2. Ändern Sie bei Bedarf die **Überwachungsdetails**. In der nachfolgenden Tabelle finden Sie weitere Details für die einzelnen bearbeitbaren Felder.

|Feld|Details|Aktion|
|---|---|---|
|Überwachungstyp|Die Zeitspanne, innerhalb der eine Antwort vom Gerät erwartet wird. Das System verwendet standardmäßig einen Service-Ping. Ein langsamer Ping wartet fünf Sekunden auf eine Antwort, was Servern, die für netzfremde Tasks optimiert sind, mehr Zeit bei der Verarbeitung der Anforderung einräumt. Ein Service-Ping setzt alle fünf Minuten einen Ping ab und erwartet innerhalb von einer Sekunde eine Echoantwort. Wenn mehr als ein Ping verpasst wird, wird ein Alert ausgegeben.|Wählen Sie zwischen **Langsamer Ping** oder **Service-Ping** aus.|
|Benachrichtigen| Benachrichtige Benutzer empfangen jedes Mal automatisierte Benachrichtigungen, wenn ein Gerät nicht in der angegebenen Antwortzeit auf einen Ping reagiert. Um Benachrichtigungen zu erhalten, muss ein Benutzer zu dem Konto gehören, das dem Gerät zugeordnet ist.|Um einen Benutzer hinzuzufügen, wählen Sie den neuen **berechtigten Benutzer** aus und klicken Sie auf **Benutzer hinzufügen**. Um einen Benutzer zu entfernen, klicken Sie neben dem vorhandenen benachrichtigten Benutzer auf das Symbol **Entfernen** und anschließend auf **Ja**, um die Aktion zu bestätigen.|
|Benachrichtigen Wartezeit|Die Zeit, die das System wartet, um eine Benachrichtigung zu senden, wenn das Gerät nicht auf das Pingsignal reagiert hat. Es stehen mehrere Wartezeiten zur Verfügung. **Hinweis:** Benachrichtigungsdetails sind nicht erforderlich, wenn keine Benutzer zur Benachrichtigung ausgewählt sind. |Wählen Sie die gewünschte Wartezeit aus.|

3. Klicken Sie auf **Aktualisieren**, um die Änderungen auf die Überwachung anzuwenden. Klicken Sie auf **Abbrechen**, um die Aktion abzubrechen.

## Nächste Schritte

Wenn eine Überwachung bearbeitet wird, funktioniert die Überwachung weiterhin, wie in den Überwachungsdetails angegeben. Wenn der Typ geändert wird, ändert sich auch die Zeitdauer für den Empfang des erwarteten Pingsignals. Wenn Benachrichtigungsoptionen geändert werden, wird der Benachrichtigungsmodus basierend auf der neuen Auswahl geändert. Die Überwachung bleibt über die Registerkarte für die Überwachung zugänglich.
