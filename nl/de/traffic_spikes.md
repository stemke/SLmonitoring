---

copyright:
  years: 2014, 2018
lastupdated: "2018-11-16"

keywords:

subcollection: slautoscale

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Wöchentliche Datenverkehrsspitzen mit der zeitplanbasierten Skalierung von Auto Scale verwalten
{: #managing-weekly-traffic-spikes-with-auto-scale-schedule-based-scaling}

Leistungsspitzen beim Webdatenverkehr können positiv und zugleich negativ sein. Spitzen sind insofern positiv, als sie bedeuten, dass mehr Menschen Ihre Seite benutzen; sie können jedoch negativ sein, weil ein plötzlicher Anstieg der Aktivität Ihre Antwortzeiten beeinträchtigen kann. Mit Auto Scale können Sie Ihre Server automatisch vertikal nach oben (Scale-up) oder nach unten (Scale-down) skalieren, sodass sie Ihren geschäftlichen Anforderungen Rechnung tragen. Ein Beispiel dafür, wie die automatische Skalierung mit Auto Scale zur Steuerung von Datenverkehrsspitzen eingesetzt werden kann, ist die zeitplanbasierte Skalierung. In diesem Szenario treten bei einer sozialen Website in Dallas, Texas (USA), an den Wochenenden Lastspitzen auf. Für die Site werden von Montag bis Freitag jeweils mindestens zwei virtuelle Server benötigt. Jedes Wochenende sind jedoch zwei weitere Server erforderlich, um den verstärkten Datenverkehr bewältigen zu können. In den folgenden Schritten wird erläutert, wie Sie Auto Scale zur Unterstützung der zeitplanbasierten Skalierung einrichten.

## Gruppe für die automatische Skalierung hinzufügen
{: #add-auto-scale-group}

1. Melden Sie sich am [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} mit den eindeutigen Berechtigungsnachweisen an.
2. Wählen Sie **Services > Auto Scale > Auto Scale-Gruppe hinzufügen** aus.
3. Richten Sie eine Auto Scale-Gruppe ein, indem Sie bei **Gruppenname** einen Namen für die Gruppe eingeben, wie zum Beispiel 'Scale-up Wochenende - Gruppe'. Wählen Sie die Region und das Rechenzentrum aus.
4. Wählen Sie die Beendigungsrichtlinie für die Server aus. Wenn Sie beispielsweise **Älteste/r/s** auswählen, wird beim vertikalen Skalieren mit Scale-Down der Server mit dem ältesten Bereitstellungsdatum ausgewählt.
5. Geben Sie an, ob es sich bei Ihrer Gruppe um eine Multi-VLAN-Skalierungsgruppe handelt und wie die vertikale Skalierung per Scale-down für die konfigurierten VLAN-Paare ausgeglichen werden soll.
6. Wählen Sie die öffentlichen und privaten VLANs aus, auf denen Ihre Server bereitgestellt werden sollen. Wenn der Zugriff auf die Server auch über das öffentliche Internet möglich sein soll (wenn auf dem VLAN Web-Server ausgeführt werden), wählen Sie das Kontrollkästchen **Nur privates Netz** nicht aus.
7. Legen Sie für **Mindestanzahl von Mitgliedern** 2 und für **Höchstanzahl von Mitgliedern** 4 fest. Legen Sie für die **Ruhephase** 0 fest. Da hier die zeitplanbasierte Skalierung verwendet wird, werden keine Statistikdaten zum Auslösen von Skalierungsaktionen erfasst.

## Mitgliedskonfiguration für Gruppe definieren
{: #define-member-configuration}

1. Suchen Sie **Mitgliedskonfiguration** und geben Sie **Hostname** und **Domäne** für den Skalierungsserver ein. Bei Servern, die nachfolgend zu der Gruppe hinzugefügt wurden, wird jeweils ein eindeutiges Suffix an den Hostnamen angehängt.
2. Geben Sie die Hardwarekonfiguration der Datenverarbeitungsinstanzen an (Kerne, RAM usw.).
3. Wählen Sie ein Betriebssystem aus, wenn Sie das minimale Betriebssystem installieren möchten. Für die Bereitstellung Ihrer Instanzen können Sie auch ein öffentliches Image oder ein privates Image verwenden.
4. Wenn für die Instanzen zusätzliche Schritte zum Installieren zusätzlicher Software erforderlich sind, geben Sie die URL für ein Nachinstallationsscript zum Installieren der Software an. (Wenn Sie ein Lastausgleichsfunktion für die Gruppe verwenden, werden die Nachinstallationsscripts ausgeführt, bevor ein Mitglieder hinter eine Lastausgleichsfunktion platziert wird.)

## Richtlinien einrichten
{: #set-up-policies}

In diesem Szenario verwendet die soziale Website eine zeitplanbasierte Skalierung. Es werden zwei Richtlinien benötigt: eine für das Scale-up der Server (vertikale Skalierung nach oben) an Freitagnachmittagen und eine zweite, um Sonntagabends ein Scale-down der Server durchzuführen. Mit der ersten Richtlinie wird ein Scale-up der Server durchgeführt.

1. Suchen Sie **Richtlinien** und klicken Sie auf **Richtlinie hinzufügen**. Geben Sie bei **Richtlinienname** den Namen für die Richtlinie ein: (Scale-up Freitag).
2. Wählen Sie für **Ruhephase** die Option 'Ruhephase für Gruppe' aus.
3. Klicken Sie auf **Auslöser hinzufügen** und geben Sie einen wiederkehrenden Auslöser an, indem Sie im ersten Dropdown-Menü den Eintrag **Alle** und in den nachfolgenden Dropdown-Menüs die Einträge **Freitag** sowie **2:00 PM**\* auswählen. (Das Kontrollkästchen **Erweiterte Bearbeitung** ermöglicht die Eingabe der Auslösehäufigkeit in Crontab–ähnlicher Schreibweise.)
4. Klicken Sie unter **Aktion** auf die Dropdown-Liste **Skalieren um** und wählen Sie **Relativ** aus. Geben Sie im Feld **Mitglieder** den Wert 2 ein.
5. Klicken Sie erneut auf **Richtlinie hinzufügen**, um die zweite Richtlinie anzugeben, mit der jeden Sonntagabend ein Scale-down der Server durchgeführt wird. Die Ruhephase entspricht der Ruhephase für die Gruppe. 'Als Auslöser ist jeder Sonntag um 1:00 AM* mit einer relativen Skalierungsaktion von -2 definiert.
6. Die Zeit, die Sie im Feld **Auslöser** eingeben, basiert auf UTC-Zeit. Daher müssen Sie 10:00 PM für 05:00 PM Central Daylight Time und 01:00 AM für 08:00 PM Central Daylight Time auswählen. Während der Central Standard Time würden die Zeitangaben 09:00 AM und 12:00 AM lauten, da UTC/GMT keine Sommerzeit berücksichtigt. Auf der Website [World Time Server ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://www.worldtimeserver.com/current_time_in_UTC.aspx){: new_window} finden Sie eine Zeitumrechnungsfunktion.

## Lokale Lastausgleichsfunktion hinzufügen

Wenn Sie über eine eingerichtete lokale Lastausgleichsfunktion verfügen, können Sie sie für den Lastausgleich in Ihrer Auto Scale-Gruppe verwenden.

1. Suchen Sie nach **Lokale Lastausgleichsfunktionen** und klicken Sie auf **Lastausgleichsfunktion hinzufügen**.
2. Klicken Sie auf **VIP-Einstellungen anzeigen**. Es wird eine neue Seite geöffnet, auf der die lokalen Lastausgleichsfunktionen angezeigt werden, die in Ihrem Konto verfügbar sind. Hier können Sie bei Bedarf auch eine neue Lastausgleichsfunktion bestellen. Einer Lastausgleichsfunktion muss eine Servicegruppe zugeordnet sein, die mit einer Auto Scale-Gruppe verwendet werden soll. Stellen Sie sicher, dass sich die Lastausgleichsfunktion im Rechnungszentrum Ihrer Auto Scale-Gruppe befindet.
3. Klicken Sie auf der Seite **Auto Scale-Gruppe hinzufügen** auf **Lastausgleichsfunktion hinzufügen**, klicken Sie dann auf den Dropdown-Pfeil für 'Virtuelle IP' und wählen Sie Ihre Lastausgleichsfunktion aus.
4. Klicken Sie auf die Dropdown-Pfeile für **Servicegruppe**, **Service-Port** und **Typ der Servicestatusprüfung** und wählen Sie die entsprechenden Werte aus.
5. Klicken Sie auf **Gruppe hinzufügen**, um Ihre Gruppe zu speichern.
6. Wenn Sie alle Datencenter, Netzwerke usw. richtig angegeben haben, wird Ihre Auto Scale-Gruppe erstellt. Klicken Sie auf die Gruppe in der Anzeige **Alle Gruppen anzeigen**, um die Gruppendetails anzuzeigen.

Die Einrichtung einer zeitplanbasierten Skalierung hat zum Ergebnis, dass zwei Mitglieder automatisch bereitgestellt werden, um so die Mindestanforderungen der Website zu erfüllen. Freitags werden um 5:00 PM Central Time automatisch zwei weitere Mitglieder bereitgestellt, wenn der erste Richtlinienauslöser zur Anwendung kommt. Sonntags um 8:00 PM Central Time werden durch Auslösen der zweiten Richtlinie zwei Mitglieder wieder zurückgefordert. Bei Angabe einer Lastausgleichsfunktion befinden sich alle Mitglieder, die bei der Erstellung oder am Freitag erstellt wurden, hinter der Lastausgleichsfunktion, nachdem das benutzerdefinierte Nachinstallationsscript ausgeführt worden ist.
