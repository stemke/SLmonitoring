---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Nimsoft Monitoring-Agentenbericht konfigurieren
{: #configuring-a-nimsoft-monitoring-agent-report}

## Vorbereitungen

Navigieren Sie zuerst zum Gerätemenü und stellen Sie sicher, dass Sie über die korrekten Kontoberechtigungen verfügen, um die Tasks auszuführen.

* Navigieren Sie zum Gerätemenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Geräten navigieren](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Stellen Sie sicher, dass Sie über alle erforderlichen Kontoberechtigungen und Gerätezugriffe verfügen. Nur der Kontoeigner oder ein Benutzer mit der klassischen Infrastrukturberechtigung **Manage Users** (Benutzer verwalten) kann die Berechtigungen anpassen.

Weitere Informationen zu Berechtigungen finden Sie unter [Klassische Infrastrukturberechtigungen](/docs/iam?topic=iam-infrapermission#infrapermission) und [Gerätezugriff verwalten](/docs/vsi?topic=virtual-servers-managing-device-access).

## Nimsoft Monitoring-Agentenbericht konfigurieren
{: #configuring-nimsoft-monitoring-agent-report-steps}

Führen Sie die folgenden Schritte aus, um einen Nimsoft Monitoring-Agentenbericht zu konfigurieren.

1. Wählen Sie im Menü **Geräte** die Option **Überwachung** aus.
2. Wählen Sie auf der Seite **Überwachung** die Option **Agentenberichte konfigurieren** aus dem Dropdown-Menü **Aktionen** in der Spalte **Erweitert** aus.
3. Wählen Sie den zu konfigurierenden Agenten aus der Dropdown-Liste **Agenten** aus.
  
  Die verfügbaren Agenten sind je nach Gerät anders und hängen von dem Überwachungspaket ab, das auf das Gerät angewendet wurde.
  {:note}

4. Wählen Sie den zu konfigurierenden Abschnitt aus der Dropdown-Liste **Abschnitt** aus. Wenn Sie einen Abschnitt auswählen, der Profile enthält, wird eine weitere Dropdown-Liste angezeigt. Wählen Sie aus dieser Liste ein **vorhandenes Profil** aus der Dropdown-Liste **Profile** aus. Um eine neue Konfiguration hinzuzufügen, wählen Sie **Agentenkonfiguration hinzufügen...** aus der Dropdown-Liste **Profile** aus.

5. Füllen Sie bei Bedarf alle Felder im Abschnitt **Allgemeine Metriken und Informationen** aus.
  
  Erforderliche Felder sind durch einen roten Stern (*) gekennzeichnet. Nicht alle Agenten, Abschnitte oder Profile enthalten diesen Abschnitt.
  {:note}

6. Aktivieren Sie bei Bedarf das Kontrollkästchen **Metrik** für jede einzuschließende Metrik im Abschnitt zum **Auswählen von zu dokumentierenden Metriken**.

7. Aktivieren Sie das Kontrollkästchen **Alarm** für jeden für den Agenten zu aktivierenden Alarm unter **Metrikalarme**.

  Nicht alle Alarme in diesem Abschnitt sind an eine bestimmte Metrik gebunden. Alarme werden an alle E-Mail-Adressen gesendet, die dem Abschnitt mit den **Alarmabonnenten** für den Agenten zugeordnet sind.
  {:note}

7. Klicken Sie auf **Speichern**, um die Konfiguration zu speichern. Klicken Sie auf **Abbrechen**, um die Aktion abzubrechen.
  
  Die Schaltfläche **Speichern** ist so lange inaktiviert, bis Sie die aktuelle Konfiguration ändern.
  {:note}

## Nächste Schritte

Nachdem Sie die Konfiguration erfolgreich gespeichert haben, wird eine Bestätigungsnachricht angezeigt. Wenn die Konfiguration nicht erfolgreich war, wird eine Fehlernachricht mit Details zu dem aufgetretenen Fehler sowie eine Lösungsmöglichkeit angezeigt. Durch Wiederholen dieser Schritte können Sie Agenten jederzeit neu konfigurieren.
