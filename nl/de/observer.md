Ein Administrator erhält eine ganzheitliche Übersicht über den aktuellen und früheren Zustand seines Geräts an einem Ort.

Benutzerstorys:

    Jeder Benutzer kann für die Registerkarten 'Bandbreite' und 'Nutzung' schnell zwischen der vorhandenen Ansicht und der Observer-Betaversion (nur BETA) umschalten.

    Jeder Benutzer kann Feedback zu seinen Erfahrungen in der Observer-Betaversion über das Steuerungsportal (nur BETA) geben.

    Jeder Benutzer hat Zugriff auf die Blogbeiträge, um mehr zu unserer Arbeit an Observer in der Betaversion zu erfahren (nur BETA).

    Benutzern steht eine bestimmte Position zur Verfügung, an der sie Metriken zu Infrastrukturressourceen für virtuelle Server speichern und anzeigen können:

    1. CPU-Auslastung, %, pro virtueller Kern

    2. Öffentliches Netz, eingehend/abgehend, Byte und Pakete

    3. Privates Netz, eingehend/abgehend, Byte und Pakete

    4. Speicherauslastung, %

    5. Lesevorgänge Platte, Byte und Operationen

    6. Schreibvorgänge Platte, Byte und Operationen

    7. Übertragung von Fehlern, eingehend/abgehend, Anzahl

    8. Latenz Platte, Millisekunde, Lese- und Schreibvorgänge

    9. Lokale Plattennutzung, % und verwendete Byte und insgesamt verfügbare Byte


    Benutzer von Bare-Metal-Instanzen können die folgenden Metriken anzeigen:

    1. CPU-Auslastung, %, pro virtueller Kern

    2. Öffentliches Netz, eingehend/abgehend, Byte und Pakete

    3. Privates Netz, eingehend/abgehend, Byte und Pakete

    4. Speicherauslastung, %

    5. Lesevorgänge Platte, Byte und Operationen

    6. Schreibvorgänge Platte, Byte und Operationen

    7. Übertragung von Fehlern, eingehend/abgehend, Anzahl

    8. Latenz Platte, Millisekunde, Lese- und Schreibvorgänge

    9. Lokale Plattennutzung, % und verwendete Byte und insgesamt verfügbare Byte

    10. RAID-Alerts, 0/1

    11. Kerntemperatur, Grad Fahrenheit

    Jeder Administrator kann Protokolle für Alarme und Metriken in einer einzigen Ansicht anzeigen, ohne eine Protokollanalyse durchführen zu müssen (ähnlich wie Nr. 60).

    Ein Manager kann den allgemeinen Status eines Geräts verstehen, ohne eine Erläuterung dazu von seinem Administrationsteam erhalten zu müssen.

    Ein Benutzer kann die aktuelle syslog-Datei eines Geräts öffnen, ohne dabei die Befehlszeile zu verwenden (ähnlich wie Nr. 35).

    Ein Benutzer kann jederzeit Metrikdaten von Serien in einer Reihe von interaktiven Diagrammen anzeigen und untersuchen.

    Jeder Benutzer kann Alertprotokolle anzeigen und diese grundlegend verstehen.

    Jeder Benutzer kann Ereignisse als 'offen' oder 'geschlossen' markieren.

    Kein Benutzer muss beim Auslösen eines Alarms manuell ein Ereignis erstellen.

    Kein Benutzer muss neben den eigenen Alarmeinstellungen manuell die Bewertungsstufe 'Warnung' oder 'Fehler' zuweisen.

    Jeder Benutzer kann mithilfe von collectD-Agenten Metriken auf System- und Anwendungsebene für Überwachungsprozesse, Apache, Tomcat, MSSQL, MySQL und URL-Antworten erfassen.

    Ein Administrator kann angepasste Metrikdaten in automatisierter Art und Weise an den Überwachungsservice senden.

    Jeder Benutzer kann System-, Anwendungs- oder angepasste Metriken in der gleichen Art und Weise wie Hypervisor-Metriken verwenden: Diagramme, Dashboards, Alarme, Benachrichtigungen, automatische Antworten, Vorlagen usw.



Hill 2: Ein Administrator kann einen Vorfall innerhalb von 90 Sekunden verstehen und mit der Fehlerbehebung beginnen.

Benutzerstorys:

    Jeder Administrator kann Alerts abonnieren, ohne dabei mit falschen Alarmen überschwemmt zu werden.

    Jeder Administrator kann Alerts über seinen bevorzugten Kommunikationskanal innerhalb einer Minute nach Auslösen eines Ereignisses empfangen.

    Zuverlässigkeitstechniker können die Ursache für einen Vorfall basierend auf der Nachricht im Alert selbst verstehen.

    Jeder Administrator kann aktuelle Nutzungsmetriken für jedes beliebige Gerät mit einem hohen Grad an Genauigkeit überprüfen.

    Jeder Administrator kann unter 10 Sekunden nach von ihm benötigten Informationen suchen.

    Ein Benutzer ohne Administratorberechtigungen kann einen eskalierten Vorfall mit weniger als drei Nachrichten vom SL-Support lösen.

    Jeder Benutzer kann eine Bedingung für das Ausschalten des Alerts für eine beliebige verfügbare Metrik angeben (Standard, collectD oder angepasst).

    Jeder Benutzer kann eine Bedingung basierend auf dem Durchschnittswert, kumulativen Wert, Mindestwert oder Maximalwert einer Metrik angeben.

    Jeder Benutzer kann eine Bedingung mit der Qualifikation 'größer als' oder 'kleiner als' angeben.

    Jeder Benutzer kann die Anzahl der aufeinanderfolgenden Perioden angeben, für die eine Bedingung erfüllt sein muss, sowie die Länge der Periode (entweder 30 Sekunden oder 5 Minuten), bevor ein Alarm ausgelöst wird: 'Wenn X für 2 aufeinanderfolgende Perioden von 30 Sekunden auftritt, wird der Alarm ausgelöst'.

    Jeder Benutzer kann mehrere Bedingungen für einen einzelnen Alarm angeben: 'Falls dies UND dies UND dies, wird der Alarm ausgelöst'.

    Jeder Benutzer kann einen angepassten Namen für den Alarm angeben.

    Jeder Benutzer kann über Alerts informiert werden, die den Zeitpunkt, den Alarmnamen und die Bedingungen enthalten, die zum Auslösen des entsprechenden Alarms geführt haben.

    Ein Benutzer erhält nach dem Auslösen eines Alarms erst dann weitere Alerts von derselben Regel für dasselbe Gerät, wenn der ursprüngliche Alarm 'geschlossen' wurde.

    Beispiel für Alarmregel: Wenn die durchschnittliche CPU-Auslastung für 2 aufeinanderfolgende Perioden von 5 Minuten bei über 80 % liegt UND die Summe des eingehenden Netzverkehrs höher als 50 GB/s für 1 aufeinanderfolgende Periode von 5 Minuten ist, wird ein Alarm ausgelöst und ein Ereignis erstellt (unter der Annahme, dass alle vorherigen Alarme von dieser Regel geschlossen wurden).

    Ein Administrator kann 1 oder mehrere E-Mail-Adressen zur Benachrichtigung von Benutzern angeben.

    Ein Administrator kann 1 oder mehrere Telefonnummern für SMS zur Benachrichtigung von Benutzern angeben.

    Ein Administrator kann 1 oder mehrere URLs für zu sendende Webhooks angeben.

    Ein Administrator kann eine PagerDuty-Gruppe zur Benachrichtigung von Benutzern angeben.

    Ein Administrator kann angeben, ob der Server beim Auslösen des Alarms neu gestartet oder heruntergefahren werden soll.

    Ein Administrator kann ein Intervall von 30 Sekunden oder 5 Minuten für die Netzüberwachung eines unterstützten Protokolls angeben.

    Ein Administrator kann Host-Ping-Überprüfungen (ICMP) implementieren.

    Ein Administrator kann Überprüfungen von TCP-Ports für verschiedenen Protokolle implementieren: DNS, DNS Custom, FTP, HTTP, HTTP Custom, HTTPS, IMAP, LDAP, NNTP, POP, SMTP, SSH, TCP Custom, TELNET, UDP SIP (Unterstützung für diese Protokolle ist in aktuellen SL TCP-Angeboten vorhanden).

    Ein Administrator kann eine Überprüfung eines TCP-Ports für das SNMP-Protokoll implementieren (aktuell nicht im vorhandenen SL-Angebot unterstützt).

    Ein Administrator kann einen Schwellenwert für eine Antwortzeit angeben, der über die Einordnung als Erfolg oder Fehler entscheidet.

    Ein Administrator kann die Anzahl der aufeinanderfolgenden Fehler von einem Host-Ping oder einer TCP-Portüberprüfung angeben, bevor ein Alarm ausgelöst wird.

    Ein Administrator kann dieselben Optionen für Benachrichtigungen und automatische Antwortzeiten von Netzüberwachungsalarme wie von auf Metriken basierenden Alarmen (E-Mail, SMS, Webhook, PagerDuty, Neustart, Herunterfahren) implementieren.

    Ein Administrator kann die Bewertungsstufen 'Warnung' oder 'Fehler' sowohl für Metrik- als auch für Netzüberwachungsalarme angeben.



Hill 3: Jeder Benutzer kann eine Überwachung auf einem beliebigen Gerät einrichten und dabei weniger als 90 Sekunden für Konfigurationsentscheidungen benötigen (ähnlich wie Nr. 59).

Benutzerstorys:

    Ein Benutzer ohne Administratorberechtigungen kann die Überwachung nur über die Schnittstelle und mithilfe der entsprechenden Dokumentation konfigurieren.

    Ein Administrator kann eine Überwachung einrichten, die seinen spezifischen Anforderungen entspricht, indem er gespeicherte oder vordefinierte Konfigurationen auswählt, ohne dabei den manuellen Konfigurationsprozess durchlaufen zu müssen (ähnlich wie Nr. 58).

    Ein Administrator kann eine Überwachung einrichten, die seinen spezifischen Anforderungen entspricht, indem er eine Konfiguration manuell bearbeitet und speichert und diese auf eine beliebige Anzahl von Geräten anwendet.

    Ein Administrator kann Alerts für mehrere Geräte mit minimal wiederkehrendem Aufwand einrichten.

    Jeder Benutzer kann zeit- und metrikspezifische Daten in eine CSV-Datei exportieren.

    Ein Administrator oder Manager kann ein Wartungsfenster einrichten, in dessen Zeitrahmen beim Auslösen von Alarmen keine Benachrichtigungen gesendet werden.

    Jeder eingerichtete Benutzer kann gespeicherte Konfigurationen verstehen und anwenden (ähnlich wie Nr. 41).

    Jeder neue Benutzer kann vordefinierte Konfigurationen verstehen und anwenden (ähnlich wie Nr. 34, Nr. 32).

    Ein Benutzer ohne Administratorberechtigungen kann Unterstützung bei der Einrichtung der Überwachung erhalten, ohne dass er ein Support-Ticket anlegen muss.

    Jeder Kunde kann ohne Fachwissen für jedes Gerät eine Überwachung bestellen (ähnlich wie Nr. 63, Nr. 43).

    Alle Kunden verfügen über eine einheitliche, einschätzbare Erfahrung bei der Bestellung einer Überwachung für ein beliebiges Gerät (ähnlich wie Nr. 40).

    Jeder Benutzer kann sein Gerät mit einem Service eines Drittanbieters integrieren, ohne ein Support-Ticket anlegen zu müssen.

    Kein Benutzer muss manuell einen Alarm für Warnungsalerts im Lebenszyklus erstellen: Erstellen, Booten, Herunterfahren.

    Jeder technische Benutzer kann auf alle Observer-Funktionen über dieselbe API wie der Rest des Überwachungsservice zugreifen.

    IBM kann den Zugriff von AB-Konten auf bestimmte Funktionen/die Leistung mit der kostenlosen Version einschränken, wie in der Observer-Übersicht zu den Vor- und Nachteilen von kostenlosen und kostenpflichtigen Tiers definiert.

    Jeder Kunde kann über die Registerkarte 'Überwachung' ein Upgrade von einer kostenlosen auf eine kostenpflichtige Version durchführen.

    Jeder Kunden kann im Bereich für die Kontoverwaltung ein Upgrade oder Downgrade von kostenpflichtigen oder kostenlosen Versionen durchführen.

    Jeder Benutzer der kostenlosen Version kann die Optionen anzeigen, die bei einem Upgrade zur Verfügung stehen würden: jedoch wird auch angegeben, warum diese nicht verfügbar sind.

    Wenn ein Benutzer versucht, eine Aktion durchzuführen, für die ein Upgrade erforderlich wäre, sollte eine Nachricht angezeigt werden, die angibt, dass ein Upgrade erforderlich ist und außerdem eine mögliche Alternative anbietet (z. B. 'Sie verfügen bereits über die maximale Anzahl an Alarmen für die kostenlose Version. Führen Sie ein Upgrade durch oder löschen Sie einen Alarm, um eine neue Regel zu erstellen').


