---

copyright:
  years: 2014, 2018
lastupdated: "2018-03-01"

keywords:

subcollection: slautoscale

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Datenverkehrsspitzen mit der ressourcenbasierten Skalierung von Auto Scale verwalten
{: #managing-traffic-spikes-with-auto-scale-resource-based-scaling}

Die Einführung eines neuen Produkts oder verkaufsfördernde Maßnahmen für ein vorhandenes Produkt können auf Ihrer Website zu Lastspitzen durch starken Datenverkehr führen. Eine Lastspitze im Datenverkehr kann sich nachteilig auf Ihre Antwortzeit auswirken, was seinerseits das Erlebnis Ihrer Kunden auf Ihrer Website beeinträchtigt. {{site.data.keyword.cloud}} Auto Scale ermöglicht Ihnen, automatisch auf Datenverkehrsspitzen zu reagieren. Ein Beispiel dafür, wie die automatische Skalierung mit Auto Scale zur Steuerung von Datenverkehrsspitzen eingesetzt werden kann, ist die ressourcenbasierte Skalierung. In diesem Szenario müssen für eine E-Commerce-Site in Dallas, Texas (USA), rund um die Uhr drei virtuelle Server online sein. Bei den Geschäftsaktivitäten treten an jedem Wochentag zwischen 9:00 Uhr und 17:00 Uhr Lastspitzen auf, wenn das Unternehmen Onlineverkäufe abhält. Um die Antwortzeiten der Website weiterhin aufrechterhalten zu können, sind in dieser Zeit jeweils drei zusätzliche virtuelle Server erforderlich. Wenn der öffentliche eingehende Datenverkehr über einen Zeitraum von 10 Minuten auf allen virtuellen Servern einen Durchschnittswert von über 5 MB pro Sekunde erreicht, sollen zusätzlich zwei weitere virtuelle Server bereitgestellt werden. Wenn der Datenverkehr unter 5 MB pro Sekunde sinkt, sollen diese zusätzlich bereitgestellten virtuellen Server storniert und entfernt werden. Das Ziel besteht darin, dass nicht mehr als fünf virtuelle Server den Anstieg des Datenverkehrs bewältigen, wodurch die regulären virtuellen Server für die Wochentage nicht durch den zusätzlichen Datenverkehr an Wochentagen beeinträchtigt werden. In den folgenden Schritten wird erläutert, wie Sie Auto Scale zur Unterstützung der ressourcenbasierten Skalierung einrichten.

## Gruppe für die automatische Skalierung hinzufügen
{: #adding-auto-scale-group}

1. Melden Sie sich bei {{site.data.keyword.cloud_notm}} an und wählen Sie **Geräte > Auto Scale** aus. Klicken Sie auf **Auto Scale-Gruppe hinzufügen**.
2. Richten Sie eine Auto Scale-Gruppe ein, indem Sie bei **Gruppenname** einen Namen für die Gruppe eingeben, wie zum Beispiel 'Scale-up Wochenende - Gruppe'. Wählen Sie die Region und das Rechenzentrum aus.
3. Wählen Sie die Beendigungsrichtlinie für die Server aus. Wenn Sie beispielsweise **Älteste/r/s** auswählen, wird beim vertikalen Skalieren mit Scale-Down der Server mit dem ältesten Bereitstellungsdatum ausgewählt.
4. Geben Sie an, ob es sich bei Ihrer Gruppe um eine Multi-VLAN-Skalierungsgruppe handelt und wie die vertikale Skalierung per Scale-down für die konfigurierten VLAN-Paare ausgeglichen werden soll.
5. Wählen Sie die öffentlichen und privaten VLANs aus, auf denen Ihre Server bereitgestellt werden sollen. Wenn der Zugriff auf die Server auch über das öffentliche Internet möglich sein soll (wenn auf dem VLAN Web-Server ausgeführt werden), wählen Sie das Kontrollkästchen **Nur privates Netz** nicht aus.
6. Legen Sie für **Mindestanzahl von Mitgliedern** 3 und für **Höchstanzahl von Mitgliedern** 6 fest. Legen Sie für die **Ruhephase** 0 fest. Da hier die zeitplanbasierte Skalierung verwendet wird, werden keine Statistikdaten zum Auslösen von Skalierungsaktionen erfasst.

## Mitgliedskonfiguration für Gruppe definieren
{: #defining-member-configuration}

1. Suchen Sie **Mitgliedskonfiguration** und geben Sie **Hostname** und **Domäne** für den Skalierungsserver ein. Bei Servern, die nachfolgend zu der Gruppe hinzugefügt wurden, wird jeweils ein eindeutiges Suffix an den Hostnamen angehängt.
2. Geben Sie die Hardwarekonfiguration der Datenverarbeitungsinstanzen an (Kerne, RAM usw.).
3. Wählen Sie ein Betriebssystem aus, wenn Sie das minimale Betriebssystem installieren möchten. Für die Bereitstellung Ihrer Instanzen können Sie auch ein **öffentliches Image** oder ein **privates Image** verwenden.
4. Wenn für die Instanzen zusätzliche Schritte zum Installieren zusätzlicher Software erforderlich sind, geben Sie die URL für ein **Nachinstallationsscript** zum Installieren der Software an. (Wenn Sie ein Lastausgleichsfunktion für die Gruppe verwenden, werden die Nachinstallationsscripts ausgeführt, bevor ein Mitglied hinter eine Lastausgleichsfunktion platziert wird.)

## Richtlinien einrichten

In diesem Szenario verwendet die E-Commerce-Site eine ressourcenbasierte Skalierung. Es werden zwei Richtlinien benötigt: eine für eine relative Skalierung von +3 über den erforderlichen Zeitraum und eine zweite für eine Auflösungsaktion von 3, sobald die Lastspitze vorbei ist. Mit der ersten Richtlinie werden die Ressourcen hinzugefügt.

1. Blättern Sie abwärts **Richtlinien** und klicken Sie auf **Richtlinie hinzufügen**. Geben Sie bei **Richtlinienname** den Namen für die Richtlinie ein: (Scale-up Wochentag).
2. Wählen Sie für **Ruhephase** die Option 'Ruhephase für Gruppe' aus.
3. Klicken Sie auf **Auslöser hinzufügen** und geben Sie einen wiederkehrenden Auslöser an, indem Sie im ersten Dropdown-Menü den Eintrag**Alle** auswählen und in den nachfolgenden Dropdown-Listen die Einträge **Montag, Dienstag, Mittwoch, Donnerstag, Freitag** sowie ******2:00 PM**\* markieren. (Das Kontrollkästchen **Erweiterte Bearbeitung** ermöglicht die Eingabe der Auslösehäufigkeit in Crontab–ähnlicher Schreibweise.)
4. Klicken Sie unter **Aktion** auf die Dropdown-Liste **Skalieren um** und wählen Sie **Genau** aus. Geben Sie im Feld **Mitglied** den Wert 3 ein.
5. Klicken Sie erneut auf **Richtlinie hinzufügen**, um die zweite Richtlinie anzugeben, mit der jeden Nachmittag die Server wieder entfernt werden. Die Ruhephase entspricht der Ruhephase für die Gruppe. Definieren Sie für den Auslöser jeden Montag, Dienstag, Mittwoch, Donnerstag und Freitag um 10:00 PM\* mit der genauen Skalierungsaktion 3. Die Zeit, die Sie im Feld **Auslöser** eingeben, basiert auf UTC-Zeit. Daher müssen Sie 02:00 PM für 09:00 AM Central Daylight Time und 10:00 PM für 05:00 PM Central Dayliht Time auswählen. Während der Central Standard Time würden die Zeitangaben 01:00 PM und 09:00 PM lauten, da UTC/GMT keine Sommerzeit berücksichtigt. Auf der Website [World Time Server ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://www.worldtimeserver.com/current_time_in_UTC.aspx){: new_window} finden Sie eine Zeitumrechnungsfunktion.
6. Richten Sie eine weitere Gruppe mit einer Ruhephase von 0 ein. Benennen Sie sie beispielsweise 'Burst Datenverkehr - Gruppe' und ordnen Sie ihr den Wert 0 als Mindestanzahl von Mitgliedern und den Wert 5 als Höchstanzahl von Mitgliedern zu. Verwenden Sie dieselben Einstellungen für die Gruppen- und die Mitgliederkonfiguration wie für die Gruppe 'Scale-up Wochentag'.
7. Klicken Sie auf **Richtlinie hinzufügen**, um die zweite Richtlinie hinzuzufügen, die die beiden zusätzlichen Server steuert, wenn der öffentliche eingehende Datenverkehr über einen Zeitraum von 10 Minuten auf allen virtuellen Servern einen Durchschnittswert von über 5 MB pro Sekunde erreicht.
8. Geben Sie bei **Richtlinienname** einen Namen ein, zum Beispiel 'Burst Datenverkehr - Gruppe'.
9. Wählen Sie für **Ruhephase** die Option 'Ruhephase für Gruppe' aus.
10. Klicken Sie auf **Auslöser hinzufügen**. Übernehmen Sie die Standardangabe **Wenn mein** im ersten Feld unverändert und wählen Sie im zweiten Feld **Öffentliches Netz eingehend - Mbps** aus. Übernehmen Sie im dritten Feld das Standardsymbol '>'. Geben Sie im vierten Feld die Zahl **5** (5 MB) ein, geben Sie im fünften Feld den Wert **600** ein und wählen Sie im letzten Feld die Einheit **Sekunden** aus, um auf diese Art 10 Minuten anzugeben.
11. Klicken Sie unter **Aktion** auf die Dropdown-Liste **Skalieren um** und wählen Sie **Relativ** aus. Geben Sie im Feld **Mitglied** den Wert 2 ein.
12. Klicken Sie erneut auf **Richtlinie hinzufügen**, um die zweite Richtlinie anzugeben, mit der jeden Nachmittag die Server wieder entfernt werden, wenn der Datenverkehr auf unter 5 Mbps gesunken ist. \*Als Ruhephase wird derselbe Zeitraum verwendet wie für die Gruppe. Der Auslöser lautet 'Wenn im eigenen öffentlichen Netz der eingehende Datenverkehr geringer als 5 (5 Mbps) ist, und zwar über einen Zeitraum von 600 Sekunden (d. h. 10 Minuten)'.

Wenn beide Gruppen erstellt worden sind, erstellt die Gruppe 'Scale-up Wochentag' drei Server (Mindestanzahl). An Wochentagen werden um 9:00 AM Central Time drei weitere Server hinzugefügt und um 5:00 PM wieder entfernt. Es gibt keine andere Möglichkeit, Mitglieder zu dieser Gruppe hinzuzufügen oder aus dieser Gruppe zu entfernen. In einer vollständig separaten Gruppe namens 'Burst Datenverkehr - Gruppe' werden für jeden Zeitraum von 10 Minuten, über den der eingehende öffentliche Datenverkehr bei allen Mitgliedern einen Durchschnitt von 5 MB pro Sekunde erreicht, jeweils zwei Server hinzugefügt, bis die Höchstanzahl von 5 Servern für die Gruppe erreicht ist. Nachdem der eingehende öffentliche Datenverkehr diesen Wert 10 Minuten lang unteschritten hat, werden alle Server in dieser Gruppe entfernt.
