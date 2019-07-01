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

# Visualizzazione e gestione dei monitoraggi
{: #viewing-and-managing-monitors}

Il monitoraggio di un dispositivo ti consente di avviare i ping lenti e del servizio per assicurarsi che il dispositivo sia online e reattivo.
{:shortdesc}

Se non viene ricevuta una risposta echo nell'intervallo di tempo assegnato (1 secondo per i ping del servizio, 5 secondi per i ping lenti) viene inviato un avviso all'indirizzo email nell'account. Uno stato di **Up** nel campo **Status** indica che è stata ricevuta una risposta echo, mentre **Down**
indica che la risposta echo non è stata ricevuta. Se hai un monitoraggio di base configurato, attieniti alla seguente procedura per visualizzare e gestire il monitoraggio per un dispositivo.

## Prima di cominciare
Per prima cosa passa al menu del dispositivo e assicurati di disporre delle autorizzazioni account corrette per completare le attività.

* Passa al menu del dispositivo della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assicurati di avere tutte le autorizzazioni account necessarie e l'accesso al dispositivo. Solo il proprietario dell'account o un utente con l'autorizzazione dell'infrastruttura classica **Manage Users**, può modificare le autorizzazioni.

Per ulteriori informazioni sulle autorizzazioni, vedi [Autorizzazioni dell'infrastruttura classica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gestione accesso dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Visualizzazione dei monitoraggi
{: #viewing-monitors}

1. Dal menu **Devices**, seleziona **Device List**.
2. Fai clic sul nome del dispositivo per accedervi.
3. Fai clic sulla scheda **Monitoring**. Tutti i ping correnti sono visualizzabili nella pagina di destinazione.

La scheda **Monitoring** è visibile solo se è configurato almeno un monitoraggio.
{:note}

## Aggiunta di un monitoraggio
{: #adding-a-monitor}

1. Dal menu **Devices**, seleziona **Device List**.
2. Fai clic sul nome del dispositivo per accedervi.
3. Fai clic sulla scheda **Monitoring** e seleziona **Manage monitors**.
4. Seleziona **Add Monitor**.
5. Seleziona l'indirizzo IP nel campo **IP Address** e il tipo di monitoraggio nel campo **Monitor Type**. 
6. Configura le opzioni di notifica. Nel campo **Notify ?**, seleziona **Notify Users** per avvertire gli utenti dei problemi o seleziona **Do Nothing** per ignorare la notifica utente.
7. Seleziona l'intervallo di tempo per la notifica utente nel campo **Notify Wait**.
8. Fai clic su **Add Monitor** per aggiungere il monitoraggio al dispositivo. Il nuovo monitoraggio appare nella sezione **Edit Existing Monitors**.

## Modifica di un monitoraggio esistente
{: #editing-an-exisiting-monitor}

1. Dal menu **Devices**, seleziona **Device List**.
2. Fai clic sul nome del dispositivo per accedervi.
3. Fai clic sulla scheda **Monitoring** e seleziona **Manage monitors**.
4. Nella sezione **Edit Existing Monitors**, fai clic su uno qualsiasi dei dettagli del monitoraggio per aprire il monitoraggio per modificarlo.
5. Aggiorna qualsiasi campo di seguito indicato: **Monitor Type, Notify,** o **Notify Wait**.
6. Fai clic su **Update** per aggiornare i dettagli.

## Rimozione di un monitoraggio
{: #removing-a-monitor}

1. Dal menu **Devices**, seleziona **Device List**.
2. Fai clic sul nome del dispositivo per accedervi.
3. Fai clic sulla scheda **Monitoring** e seleziona **Manage monitors**.
4. Nella sezione **Edit Existing Monitors**, fai clic sull'icona **Remove** nei dettagli del monitoraggio.
5. Seleziona **Yes** per rimuovere il monitoraggio.

## Passi successivi

- Se viene aggiunto un nuovo monitoraggio, esso compare nella scheda **Monitoring**. Il monitoraggio invia un ping al dispositivo ogni 5 minuti, aspettando una risposta basata sul tipo di ping selezionato. Se la risposta prevista non viene ricevuta, viene inviata una email all'indirizzo email di notifica per l'account nell'intervallo di tempo specificato, se la notifica è selezionata.
- Se viene modificato, un monitoraggio continua a funzionare come specificato nei dettagli del monitoraggio. Se viene modificato il tipo, la quantità di tempo per ricevere il ping previsto è differente. Se le opzioni di notifica hanno subito modifiche, il modo in cui agli utenti viene notificato un tentativo non riuscito viene modificato in base alle nuove selezioni. Il monitoraggio rimane accessibile dalla scheda **Monitoring**.
- Se viene rimosso, il monitoraggio non funziona più per il dispositivo. Tutto il monitoraggio associato al monitoraggio rimosso viene arrestato e il monitoraggio non compare più nella scheda **Monitoring**.

