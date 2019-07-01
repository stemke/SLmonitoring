---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestione degli utenti notificati per il monitoraggio standard
{: #managing-notified-users-for-standard-monitoring}

Gli utenti notificati per il servizio di monitoraggio standard ricevono delle notifiche automatizzate ogni volta che un dispositivo non risponde a un ping nel tempo di risposta allocato. Puoi aggiungere o rimuovere utenti notificati in qualsiasi momento e gli utenti notificati devono trovarsi nell'account associato al dispositivo per ricevere una notifica. Attieniti alla seguente procedura per gestire gli utenti notificati per il servizio di monitoraggio standard.
{:shortdesc}

## Prima di cominciare
Per prima cosa passa al menu del dispositivo e assicurati di disporre delle autorizzazioni account corrette per completare le attività.

* Passa al menu del dispositivo della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assicurati di avere tutte le autorizzazioni account necessarie e l'accesso al dispositivo. Solo il proprietario dell'account o un utente con l'autorizzazione dell'infrastruttura classica **Manage Users**, può modificare le autorizzazioni.

Per ulteriori informazioni sulle autorizzazioni, vedi [Autorizzazioni dell'infrastruttura classica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gestione accesso dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Aggiunta di utenti notificati
{: #adding-notified-users}

Completa la seguente procedura per aggiungere gli utenti notificati al servizio di monitoraggio standard.
1. Dal menu **Device**, seleziona **Device List**.
2. Fai clic sul nome del dispositivo per accedervi.
3. Fai clic sulla scheda **Monitoring** e seleziona **Manage monitors**.
4. Seleziona **Manage Notified Users**.
5. Dall'elenco a discesa **Users to Notify**, seleziona il nuovo utente da avvisare.
6. Seleziona **Add User**.

## Rimozione degli utenti notificati
{: #removing-notified-users}

Completa la seguente procedura per rimuovere gli utenti notificati dal servizio di monitoraggio standard.
1. Dal menu **Device**, seleziona **Device List**.
2. Fai clic sul nome del dispositivo per accedervi.
3. Fai clic sulla scheda **Monitoring** e seleziona **Manage monitors**.
4. Seleziona **Manage Notified Users**.
5. Fai clic sull'icona **Remove** per rimuovere l'utente notificato esistente e seleziona quindi **Yes** per rimuovere l'utente. 

## Passi successivi

Se aggiungi un utente notificato, l'utente viene avvertito nel caso di una risposta ping mancata. Se hai rimosso un utente notificato, l'utente non riceve più una notifica relativa a una risposta ping mancata che è associata al dispositivo.
