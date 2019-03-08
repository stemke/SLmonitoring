---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Erfasste Metriken (Beta)
In diesem Abschnitt sind die für diese Beta-Überwachungsanwendung auf virtuellen und Bare-Metal-Servern erfassten Metriken aufgeführt.
{:shortdesc}

Alle hier aufgeführten Metriken sind über Grafana-Abfragen verfügbare Metriken. Weitere Informationen finden Sie in [Erweiterte Überwachungsabfrage erstellen (Beta)](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-an-advanced-monitoring-query-beta-#creating-an-advanced-monitoring-query-beta-). Diagramme stehen in der Benutzerschnittstelle nur für die folgenden Metriken zur Verfügung:
* CPU-Auslastung
* Speicherbelegung
* Lese- und Schreibvorgänge auf Platte (Byte/Sekunde und Ein-/Ausgabe pro Sekunde)
* Latenz bei Lese- und Schreibvorgängen auf Platte
* Durchsatz öffentliches Netz (eingehend/abgehend)
* Durchsatz privates Netz (eingehend/abgehend)
* Pakete öffentliches Netz (eingehend/abgehend) (nur Bare-Metal)
* Pakete privates Netz (eingehend/abgehend) (nur Bare-Metal)
* Fehler öffentliches Netz (eingehend/abgehend) (nur Bare-Metal)
* Fehler privates Netz (eingehend/abgehend) (nur Bare-Metal)
* Temperatur (nur Bare-Metal)


## CPU-Metriken
  Die CPU-Metriken messen den durchschnittlichen Prozentsatz an Zeit, die eine CPU zum Ausführen von Anweisungen während eines bestimmten Zeitraums benötigt. Der durchschnittliche Prozentsatz für Inaktivität bezieht sich auf Benutzer, Nice-Priorität, System, Wartezeit bei Ein-/Ausgabe, Hardware-Interrupts und Software-Interrupts.

## Speichermetriken
* Verwendete Byte/Verwendeter Durchschnitt: Die verwendete Speichermenge zu einem bestimmten Zeitpunkt, verfügbar in Byte und als Prozentsatz der Gesamtmenge.
* Verwendete Swap-Byte/Verwendeter Durchschnitt: Der Prozentsatz des in einem bestimmten Zeitraum verwendeten Swap-Speichers. Diese Metrik zeigt an, wie oft Sie Daten abrufen müssen, die sich nicht im Speicher befinden. Diese Metrik ist nur für Bare-Metal-Geräte verfügbar.

## Plattenmetriken

* Platte gesamt: Die Gesamtanzahl an Byte, die der Platte zur Verfügung steht. Diese Metrik sollte konstant sein.
* Belegte Platte (Byte): Die Anzahl an Byte, die von der Platte zu einem bestimmten Zeitpunkt verwendet wird.
* Belegte Platte (Prozentsatz): Der Prozentsatz der Gesamtanzahl an verwendeten Byte, die der Platte zur Verfügung steht.
* Lese-/Schreibvorgänge Platte (Byte pro Sekunde): Die durchschnittliche Menge an Daten in Byte, die in einem bestimmten Zeitraum von der/auf die Platte geschrieben/gelesen werden.
* Lese-/Schreibvorgänge Platte (Operationen pro Sekunde): Lese-/Schreiboperationen pro Sekunde.
* Lese-/Schreibvorgänge Platte (Latenz in Millisekunden pro Operation): Latenz in Millisekunden pro Lese-/Schreibvorgang.

## Netzmetriken

 * Öffentliches/Privates Netz eingehend: Anzahl der vom öffentlichen/privaten Netz gesendeten Byte.
* Öffentliches/Privates Netz abgehend: Anzahl der vom öffentlichen/privaten Netz empfangenen Byte.
* Öffentliches/Privates Netz eingehende Pakete: Anzahl der von der Netzschnittstelle im öffentlichen/privaten Netz empfangenen Pakete. Diese Metrik ist nur für Bare-Metal-Geräte verfügbar.
* Öffentliches/Privates Netz abgehende Pakete: Anzahl der von der Netzschnittstelle im öffentlichen/privaten Netz gesendeten Pakete. Diese Metrik ist nur für Bare-Metal-Geräte verfügbar.

## Temperaturmetriken
* Durchschnittstemperatur des Systems gemessen in Grad Celsius. Diese Metrik ist nur für ausgewählte Bare-Metal-Geräte verfügbar.
