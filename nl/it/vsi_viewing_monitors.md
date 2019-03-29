---

copyright:
  years: 2017
lastupdated: "2017-09-28"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Visualizzazione e gestione dei monitoraggi
{: viewing-and-managing-monitors}

Il monitoraggio di un dispositivo consente agli utenti di avviare i ping lenti e del servizio per assicurarsi che il dispositivo sia online e reattivo.
{:shortdesc}

Se non viene ricevuta una risposta echo nell'intervallo di tempo assegnato (1 secondo per i ping del servizio, 5 secondi per i ping lenti) viene inviato un avviso all'indirizzo email nell'account. Uno stato di **Up** nel campo **Status** indica che è stata ricevuta una risposta echo, mentre **Down**
indica che la risposta echo non è stata ricevuta. Se hai un monitoraggio di base configurato, attieniti alla seguente procedura per visualizzare e gestire il monitoraggio per un dispositivo.

   <table>
   <CAPTION>Tabella 1. Visualizza e gestisci il monitoraggio del dispositivo</CAPTION>
   <THEAD>
   <TR>
   <th>Se l'azione da intraprendere è ...</th>
   <th>Allora...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Visualizzare i monitoraggi</td>
   <td>
   <ol>
   <li>Dal Device List, fai clic sul nome dispositivo (<b>Device Name</b>) per accedere al dispositivo.</li>
   <li>Fai clic sulla scheda <b>Monitoring</b>. Tutti i ping correnti sono visualizzabili nella pagina di destinazione. (La scheda <b>Monitoring</b> è visibile solo se è configurato almeno un monitoraggio).</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Aggiungere un monitoraggio</td>
   <td>
   <ol>
   <li>Dalla scheda <b>Monitoring</b> della pagina Device Details, fai clic su <b>Manage Monitors</b> sul lato destro della pagina per gestire i monitoraggi associati a questo dispositivo.</li>
   <li>Nella pagina Monitors, fai clic sulla scheda <b>Add Monitor</b>.</li>
   <li>Seleziona l'indirizzo IP da monitorare dall'elenco <b>IP Address</b>.</li>
   <li>Seleziona il tipo di monitoraggio dall'elenco <b>Monitor Type</b>.</li>
   <li>Configura le opzioni di notifica. Dall'elenco <b>Notify?</b>, seleziona <b>Notify Users</b> per notificare gli utenti dei problemi oppure <b>Do Nothing</b> per tralasciare la notifica utente.</li>
   <li>Seleziona l'intervallo di tempo per la notifica utente con l'utilizzo dall'elenco <b>Notifica Aspetta</b>.</li>
   <li>Fai clic su <b>Add Monitor</b> per aggiungere il monitoraggio per il dispositivo. Il nuovo monitoraggio appare nella sezione <b>Edit Existing Monitors</b> della schermata.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Modificare un monitoraggio esistente</td>
   <td>
   <ol>
   <li>Nella pagina Monitor sotto l'intestazione <b>Edit Existing Monitors</b>, fai clic su uno qualsiasi dei dettagli del monitoraggio per aprire il monitoraggio per le modifiche.</li>
   <li>Aggiorna qualsiasi campo di seguito indicato: Monitor Type, Notify, Notify Wait.</li>
   <li>Fai clic su <b>Update</b> per aggiornare i dettagli. Fai clic su <b>Cancel</b> per annullare la modifica.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Rimuovere un monitoraggio</td>
   <td>
   <ol>
   <li>Nella pagina Monitors sotto l'intestazione <b>Edit Existing Monitors</b>, fai clic sull'icona Remove accanto ai dettagli del monitoraggio.</li>
   <li>Fai clic su <b>Yes</b> per rimuovere il monitoraggio. Fai clic su <b>No</b> per annullare l'azione.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
   </table>

## Passi successivi

- Se viene aggiunto un nuovo monitoraggio, esso compare nella scheda **Monitoring**. Il monitoraggio invia un ping al dispositivo ogni 5 minuti, aspettando una risposta basata sul tipo di ping selezionato. Se la risposta prevista non viene ricevuta, viene inviata una email all'indirizzo email di notifica per l'account nell'intervallo di tempo specificato, se la notifica è selezionata.
- Se viene modificato, un monitoraggio continua a funzionare come specificato nei dettagli del monitoraggio. Se viene modificato il tipo, la quantità di tempo per ricevere il ping previsto è differente. Se le opzioni di notifica hanno subito modifiche, il modo in cui agli utenti viene notificato un tentativo non riuscito viene modificato in base alle nuove selezioni. Il monitoraggio rimane accessibile dalla scheda **Monitoring**.
- Se viene rimosso, il monitoraggio non funziona più per il dispositivo. Tutto il monitoraggio associato al monitoraggio rimosso viene arrestato e il monitoraggio non compare più nella scheda **Monitoring**.
