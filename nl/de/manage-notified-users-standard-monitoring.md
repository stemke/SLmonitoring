---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Benachrichtige Benutzer für die Standardüberwachung verwalten
{: #managing-notified-users-for-standard-monitoring}

Benachrichtige Benutzer für den Standardüberwachungsservice empfangen jedes Mal automatisierte Benachrichtigungen, wenn ein Gerät nicht in der angegebenen Antwortzeit auf einen Ping reagiert. Sie können benachrichtigte Benutzer jederzeit hinzufügen oder entfernen und diese Benutzer müssen dem Konto angehören, das dem Gerät zugeordnet ist, um eine Benachrichtigung zu erhalten. Führen Sie die folgenden Schritte aus, um benachrichtigte Benutzer für den Standardüberwachungsservice zu verwalten.
{:shortdesc}

## Vorbereitungen
Navigieren Sie zuerst zum Gerätemenü und stellen Sie sicher, dass Sie über die korrekten Kontoberechtigungen verfügen, um die Tasks auszuführen.

* Navigieren Sie zum Gerätemenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Geräten navigieren](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Stellen Sie sicher, dass Sie über alle erforderlichen Kontoberechtigungen und Gerätezugriffe verfügen. Nur der Kontoeigner oder ein Benutzer mit der klassischen Infrastrukturberechtigung **Manage Users** (Benutzer verwalten) kann die Berechtigungen anpassen.

Weitere Informationen zu Berechtigungen finden Sie unter [Klassische Infrastrukturberechtigungen](/docs/iam?topic=iam-infrapermission#infrapermission) und [Gerätezugriff verwalten](/docs/vsi?topic=virtual-servers-managing-device-access).

## Benachrichtigte Benutzer hinzufügen
{: #adding-notified-users}

Führen Sie die folgenden Schritte aus, um benachrichtigte Benutzer für den Standardüberwachungsservice hinzuzufügen.
1. Wählen Sie im Menü **Gerät** die Option **Geräteliste** aus.
2. Klicken Sie auf den Gerätenamen, um auf das Gerät zuzugreifen.
3. Klicken Sie auf die Registerkarte **Überwachung** und wählen Sie **Überwachungen verwalten**aus.
4. Wählen Sie **Benachrichtigte Benutzer verwalten** aus.
5. Wählen Sie in der Dropdown-Liste **Zu benachrichtigende Benutzer** den neuen Benutzer aus, der benachrichtigt werden soll.
6. Wählen Sie **Benutzer hinzufügen** aus.

## Benachrichtigte Benutzer entfernen
{: #removing-notified-users}

Führen Sie die folgenden Schritte aus, um benachrichtigte Benutzer für den Standardüberwachungsservice zu entfernen.
1. Wählen Sie im Menü **Gerät** die Option **Geräteliste** aus.
2. Klicken Sie auf den Gerätenamen, um auf das Gerät zuzugreifen.
3. Klicken Sie auf die Registerkarte **Überwachung** und wählen Sie **Überwachungen verwalten**aus.
4. Wählen Sie **Benachrichtigte Benutzer verwalten** aus.
5. Klicken Sie auf das Symbol für **Entfernen**, um den vorhandenen benachrichtigten Benutzer zu entfernen, und wählen Sie dann **Ja** aus, um den Benutzer zu entfernen. 

## Nächste Schritte

Wenn Sie einen benachrichtigten Benutzer hinzufügen, wird der Benutzer im Falle einer verpassten Antwort auf ein Pingsignal benachrichtigt. Wenn Sie einen benachrichtigten Benutzer entfernen, empfängt er keine Benachrichtigung mehr bezüglich einer verpassten Reaktion auf ein Pingsignal im Zusammenhang mit dem Gerät.
