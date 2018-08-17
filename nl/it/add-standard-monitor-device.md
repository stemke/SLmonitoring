---
copyright:
  years: 1994, 2017
lastupdated: "2017-06-09"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Aggiunta e rimozione di monitoraggi

<table>
   <CAPTION>Tabella 1. Aggiunta e rimozione di monitoraggi del dispositivo</CAPTION>
   <THEAD>
   <TR>
   <th>Se l'azione da intraprendere è ...</th>
   <th>Allora...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Aggiungere un monitoraggio</td>
   <td>
   <ol>
   <li>Dalla scheda <b>Monitoring</b> della pagina Device Details, fai clic su <b>Manage Monitors</b> sul lato destro della pagina per gestire i monitoraggi associati a questo dispositivo.</li>
   <li>Nella pagina Monitors, fai clic sulla scheda <b>Add Monitor</b>.
   * **Nota:** per il monitoraggio sono disponibili indirizzi IP pubblici e privati. Ogni indirizzo IP è identificato nella scheda **Server Info**.</li>
   <li>Seleziona l'indirizzo IP da monitorare dall'elenco a discesa <b>IP Address</b>.</li>
   <li>Seleziona il tipo di monitoraggio dall'elenco a discesa <b>Monitor Type</b>.</li>
   <li>Configura le opzioni di notifica. Dall'elenco a discesa <b>Notify?</b>, seleziona <b>Notify Users</b> per notificare gli utenti di problemi oppure <b>Do Nothing</b> per tralasciare la notifica utente.</li>
   <li>Seleziona l'intervallo di tempo per una notifica utente con l'utilizzo dell'elenco a discesa <b>Attesa notifica</b>.</li>
   <li>Fai clic su <b>Add Monitor</b> per aggiungere il monitoraggio per il dispositivo. Il nuovo monitoraggio appare nella sezione <b>Edit Existing Monitors</b> della schermata.</li>
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

- Se viene aggiunto un nuovo monitoraggio, esso compare nella scheda **Monitoring**. Il monitoraggio invia un ping al dispositivo ogni 5 minuti, aspettando una risposta basata sul tipo di ping selezionato. Se la risposta prevista non viene ricevuta, viene inviata una email all'indirizzo email di notifica per l'account nell'intervallo di tempo specificato, se viene selezionata la notifica.

- Se viene rimosso, il monitoraggio non funzionerà più per il dispositivo. Tutto il monitoraggio associato al monitoraggio rimosso smette e il monitoraggio non compare più nella scheda Monitoring.
