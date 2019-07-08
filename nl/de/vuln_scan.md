---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Scans auf Sicherheitslücken
{: #vulnerability-scans}

{{site.data.keyword.cloud}} stellt in Zusammenarbeit mit Nessus Scans auf Sicherheitslücken für alle Geräte im {{site.data.keyword.cloud_notm}}-Netz bereit. Bei diesen Scans wird nach Schwachstellen bei einem Gerät gesucht und ein Bericht mit der entsprechenden Analyse, den Sicherheitsproblemen und Fixes für Ihr Hostgerät zurückgegeben. Durch das Durchführen von Scans auf Sicherheitslücken für Ihre Geräte wird sichergestellt, dass diese jederzeit sicher sind. Außerdem sind die Scans die erste zu nutzende Ressource, wenn Sie der Meinung sind, dass ein Gerät gefährdet oder beeinträchtigt ist.  Scans auf Sicherheitslücken können über die {{site.data.keyword.cloud_notm}}-Konsole für jedes Gerät durchgeführt werden, das Ihrem Konto zugeordnet ist und über eine öffentliche IP-Adresse verfügt. Scans auf Sicherheitslücken können nicht durchgeführt werden, wenn sich das Gerät nur in einem privaten Netz befindet.
{:shortdesc}

## Nessus-Sicherheitsscanner
{{site.data.keyword.cloud_notm}} stellt einen Online-Sicherheitsscanner bereit, der auf dem Open-Source-Scanning-Tool von Nessus basiert. Auf diesen Sicherheitsscanner kann über die Registerkarte 'Sicherheit' durch Klicken auf **Scanner** zugegriffen werden. Weitere Informationen finden Sie in der Veröffentlichung zum [Nessus Scanning-Tool ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://www.nessus.org/nessus/){: new_window}.

Auf der Seite **Scanner** befindet sich eine Liste der Hardware, die für das Nessus-Tool verfügbar ist, die von {{site.data.keyword.cloud_notm}} gehostet wird. Um einen Server zu scannen oder die Ergebnisse eines vorherigen Scans anzuzeigen, klicken Sie auf den Link für die Details für den Server, der überprüft werden soll. Die Seite mit den Details zur Ermittlung von Sicherheitslücken enthält eine kurze Zusammenfassung des Servers (mit dem Servernamen, der IP-Adresse für den Scan und dem Rechenzentrum, wo sich der Server befindet). Mit **Scan starten** wird der Server mit dem Nessus Scanning-Server für einen zeitnahen Scan auf Sicherheitslücken terminiert.

Nach der Serverzusammenfassung befindet sich eine Tabelle der aktuellen und bereits durchgeführten Nessus-Scans auf Sicherheitslücken. Für jeden Scan ist das Datum, an dem der Scan angefordert wurde, das Datum, an dem der Scan gestartet wurde und bei erfolgreichem Abschluss des Scans ein Link zum Nessus-Bericht aufgeführt.

Nessus-Berichte können eine der folgenden Statusangaben aufweisen:

* Scan anstehend: Der Scan wurde für das Feld mit dem Nessus-Scanner terminiert.
* Scan wird verarbeitet: Der Scan wird aktuell durchgeführt.
* Bericht wird generiert: Der Scan ist abgeschlossen und die Testergebnisse werden in einem Bericht zusammengeführt.
* Scan abgeschlossen: Der Scan wurde erfolgreich abgeschlossen und der Sicherheitslückenbericht erstellt.
* Scan abgebrochen: Der Nessus-Scan wurde manuell von einem {{site.data.keyword.cloud_notm}}-Techniker abgebrochen.

Für alle erfolgreich abgeschlossenen Nessus-Scans in dieser Tabelle kann durch Klicken auf **Bericht anzeigen** ein Bericht angezeigt werden. Der Bericht weist zwei Tabellen auf: Eine Tabelle mit Scandetails, darunter die Anzahl der gescannten Hosts, die Anzahl der offenen Sicherheitslücken (Löcher), die gefunden wurden, und die Anzahl möglicher gefundener Sicherheitslücken (Warnungen). Die zweite Tabelle enthält Informationen zu allen gefundenen Sicherheitsproblemen: den Host, auf dem die Sicherheitslücke gefunden wurde, und eine Beschreibung der möglichen Sicherheitslücke.

Das Open-Source-Tool von Nessus ist Plug-in-basiert, was bedeutet, dass beim Identifizieren von Sicherheitslücken neue Tests entwickelt werden können. {{site.data.keyword.cloud_notm}} aktualisiert das interne Nessus-Tool in regelmäßigen Abständen; ein regelmäßiges Scannen mit dem Sicherheitsscanner wird daher empfohlen, um immer die neuesten Sicherheitsbedrohungen bekämpfen zu können.

Damit der Scan erfolgreich ist, müssen Verbindungen von sowohl 173.192.255.232 als auch von 172.17.19.38 Zugriff auf den Server erhalten.
