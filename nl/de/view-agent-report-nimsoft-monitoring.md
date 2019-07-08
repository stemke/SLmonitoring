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

# Agentenbericht für Nimsoft Monitoring anzeigen
{: #viewing-an-agent-report-for-nimsoft-monitoring}

Überwachungsdetails für Nimsoft Monitoring sind in Agentenberichten verfügbar, die die entsprechenden Details gemäß der Agentenkonfiguration bereitstellen. 
{:shortdesc}

## Vorbereitungen
Navigieren Sie zuerst zum Gerätemenü und stellen Sie sicher, dass Sie über die korrekten Kontoberechtigungen verfügen, um die Tasks auszuführen.

* Navigieren Sie zum Gerätemenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Geräten navigieren](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Stellen Sie sicher, dass Sie über alle erforderlichen Kontoberechtigungen und Gerätezugriffe verfügen. Nur der Kontoeigner oder ein Benutzer mit der klassischen Infrastrukturberechtigung **Manage Users** (Benutzer verwalten) kann die Berechtigungen anpassen.

Weitere Informationen zu Berechtigungen finden Sie unter [Klassische Infrastrukturberechtigungen](/docs/iam?topic=iam-infrapermission#infrapermission) und [Gerätezugriff verwalten](/docs/vsi?topic=virtual-servers-managing-device-access).

## Agentenbericht für Nimsoft Monitoring anzeigen
{: #viewing-agent-report-nimsoft-monitoring-steps}

Führen Sie die folgenden Schritte durch, um einen Agentenbericht für Nimsoft Monitoring anzuzeigen.

1. Wählen Sie auf der Seite **Überwachung** die Option **Agentenberichte anzeigen** aus dem Menü **Aktionen** aus.
2. Wählen Sie den anzuzeigenden Agenten aus der Liste **Agenten** aus.

  Die verfügbaren Agenten sind je nach Gerät anders und hängen von dem Überwachungspaket ab, das auf das Gerät angewendet wurde.
  {:note}
  
3. Füllen Sie alle verbleibenden Abschnitte aus und führen Sie dabei mindestens eine der folgenden Aktionen aus:

  Jeder Agent ist anders und enthält nicht zwingend jeden Abschnitt oder jede Metrik. Die in dieser Anzeige verfügbaren Optionen hängen von den für den jeweiligen Agenten verfügbaren Konfigurationsoptionen ab.
  {:note}
  
  * Wählen Sie den Abschnittsbereich aus der Liste **Abschnitte** aus.
  * Wählen Sie den Zeitraum für den Bericht aus der Liste **Anzeigen nach** aus.
  * Aktivieren Sie im Abschnitt zum **Auswählen der zu dokumentierenden Metriken** das Kontrollkästchen für jede Metrik, für die ein Bericht erstellt werden soll.
    
    Nur ähnliche Metriken werden im selben Diagramm angezeigt. Wenn im Konflikt stehende Metriken ausgewählt werden, tritt nach dem Anfordern des Diagramms ein Fehler auf.
    {:note}
4. Klicken Sie auf **Diagramm zeichnen**, um das Diagramm zu zeichnen.

## Nächste Schritte

Nach dem Zeichnen des Diagramms für den Agentenbericht kann das Diagramm jederzeit durch Wiederholen dieser Schritte erneut gezeichnet werden, um andere Metriken anzuzeigen. Es gibt keine Begrenzung bei der Anzahl der Agentenberichte, die innerhalb eines bestimmten Zeitraums generiert werden können.
