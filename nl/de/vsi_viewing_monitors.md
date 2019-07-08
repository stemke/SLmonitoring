---

copyright:
  years: 2017, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:note: .note}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Überwachungen anzeigen und verwalten
{: #viewing-and-managing-monitors}

Durch die Überwachung eines Geräts können Sie Service-Pings und langsame Pings initiieren, um sicherzustellen, dass das Gerät online und betriebsbereit ist.
{:shortdesc}

Wenn im zugewiesenen Zeitrahmen (eine Sekunde für Service-Pings, fünf Sekunden für langsame Pings) kein Echo empfangen wird, wird ein Alert an die E-Mail-Adresse
im Konto gesendet. Ein aktiver Status **** im Feld **Status** zeigt an, dass ein Echo empfangen wurde, während ein inaktiver Status ****
angibt, dass kein Echo empfangen wurde. Wenn Sie eine einfache Überwachung konfiguriert haben, führen Sie die folgenden Schritte durch, um die Überwachung für ein Gerät anzuzeigen und zu verwalten.

## Vorbereitungen
Navigieren Sie zuerst zum Gerätemenü und stellen Sie sicher, dass Sie über die korrekten Kontoberechtigungen verfügen, um die Tasks auszuführen.

* Navigieren Sie zum Gerätemenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Geräten navigieren](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Stellen Sie sicher, dass Sie über alle erforderlichen Kontoberechtigungen und Gerätezugriffe verfügen. Nur der Kontoeigner oder ein Benutzer mit der klassischen Infrastrukturberechtigung **Manage Users** (Benutzer verwalten) kann die Berechtigungen anpassen.

Weitere Informationen zu Berechtigungen finden Sie unter [Klassische Infrastrukturberechtigungen](/docs/iam?topic=iam-infrapermission#infrapermission) und [Gerätezugriff verwalten](/docs/vsi?topic=virtual-servers-managing-device-access).

## Überwachungen anzeigen
{: #viewing-monitors}

1. Wählen Sie im Menü **Geräte** die Option **Geräteliste** aus.
2. Klicken Sie auf den Gerätenamen, um auf das Gerät zuzugreifen.
3. Klicken Sie auf die Registerkarte **Überwachung**. Alle aktuellen Pings können auf der Landing-Page angezeigt werden.

Die Registerkarte **Überwachung** ist nur sichtbar, wenn mindestens eine Überwachung konfiguriert ist.
{:note}

## Überwachung hinzufügen
{: #adding-a-monitor}

1. Wählen Sie im Menü **Geräte** die Option **Geräteliste** aus.
2. Klicken Sie auf den Gerätenamen, um auf das Gerät zuzugreifen.
3. Klicken Sie auf die Registerkarte **Überwachung** und wählen Sie **Überwachungen verwalten**aus.
4. Wählen Sie **Überwachung hinzufügen** aus.
5. Wählen Sie die IP-Adresse für die Überwachung im Feld **IP-Adresse** und den Überwachungstyp im Feld **Überwachungstyp** aus. 
6. Richten Sie die Benachrichtigungsoptionen ein. Wählen Sie im Feld **Benachrichtigen?** die Option **Benutzer benachrichtigen** aus, um Benutzer über Probleme zu informieren, oder wählen Sie **Nichts tun** aus, um die Benutzerbenachrichtigung zu umgehen.
7. Wählen Sie im Feld **Benachrichtigen Wartezeit** den Zeitrahmen für die Benutzerbenachrichtigung aus.
8. Klicken Sie auf **Überwachung hinzufügen**, um die Überwachung zu dem Gerät hinzuzufügen. Die neue Überwachung erscheint im Abschnitt **Vorhandene Überwachungen bearbeiten**.

## Vorhandene Überwachung bearbeiten
{: #editing-an-exisiting-monitor}

1. Wählen Sie im Menü **Geräte** die Option **Geräteliste** aus.
2. Klicken Sie auf den Gerätenamen, um auf das Gerät zuzugreifen.
3. Klicken Sie auf die Registerkarte **Überwachung** und wählen Sie **Überwachungen verwalten**aus.
4. Klicken Sie im Abschnitt **Vorhandene Überwachungen bearbeiten** auf ein beliebiges Überwachungsdetail, um die Überwachung für die Bearbeitung zu öffnen.
5. Aktualisieren Sie eines der folgenden Felder: **Überwachungstyp, Benachrichtigen** oder **Benachrichtigen Wartezeit**.
6. Klicken Sie auf **Aktualisieren**, um die Details zu aktualisieren.

## Überwachung entfernen
{: #removing-a-monitor}

1. Wählen Sie im Menü **Geräte** die Option **Geräteliste** aus.
2. Klicken Sie auf den Gerätenamen, um auf das Gerät zuzugreifen.
3. Klicken Sie auf die Registerkarte **Überwachung** und wählen Sie **Überwachungen verwalten**aus.
4. Klicken Sie im Abschnitt **Vorhandene Überwachungen bearbeiten** bei den Überwachungsdetails auf das Symbol für **Entfernen**.
5. Klicken Sie auf **Ja**, um die Überwachung zu entfernen.

## Nächste Schritte

- Wenn eine neue Überwachung hinzugefügt wird, wird die Überwachung auf der Registerkarte **Überwachung** angezeigt. Die Überwachung sendet jede fünf Minuten einen Ping an das Gerät und erwartet basierend auf dem ausgewählten Pingtyp eine entsprechende Antwort. Wird die erwartete Antwort nicht empfangen, wird im angegebenen Zeitrahmen eine E-Mail an die Benachrichtigungs-E-Mail-Adresse für das Konto gesendet, wenn die Benachrichtigungsoption ausgewählt ist.
- Wenn eine Überwachung bearbeitet wird, funktioniert die Überwachung weiterhin, wie in den Überwachungsdetails angegeben. Wenn der Typ geändert wird, ändert sich auch die Zeitdauer für den Empfang des erwarteten Pingsignals. Wenn die Benachrichtigungsoptionen geändert werden, ändert sich basierend auf der neuen Auswahl die Art und Weise, wie Benutzer über einen fehlgeschlagenen Versuch benachrichtigt werden. Die Überwachung bleibt über die Registerkarte **Überwachung** zugänglich.
- Wenn eine Überwachung entfernt wird, funktioniert die Überwachung für das Gerät nicht mehr. Alle Überwachungsvorgänge, die mit der entfernten Überwachung verknüpft sind, werden gestoppt und und die Überwachung wird nicht mehr auf der Registerkarte **Überwachung** angezeigt.

