---
copyright:
  years: 2018
lastupdated: "2018-05-18"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creazione e gestione delle notifiche di monitoraggio (Beta)
Una notifica descrive il metodo e i dettagli utilizzati per notificare quando viene attivato un avviso. Ad esempio, per ottenere una notifica di avvertenza e una notifica di errore per una metrica, definisci una regola che monitora la soglia di avvertenza e definisci una regola che monitora la soglia di errore.
{:shortdesc} 

## Crea una notifica
 
 1. Dopo che hai aderito al programma beta, seleziona **Devices -> Monitoring**. 
 2. Fai clic sulla scheda **Notifications**.
 3. Fai clic su **Create Notification**.
 4. Immetti le informazioni per la tua nuova notifica. 

<table>
  <caption>Dettagli della notifica email</caption>
  <tr>
     <th>Campo</th>
     <th>Descrizione</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Un identificativo univoco della notifica. Questo campo è obbligatorio.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Seleziona **Email**</td>
  </tr>
  <tr>
    <td>Email Address</td>
    <td>Immetti l'indirizzo email del destinatario.</td>
  </tr>
</table>

<table>
  <caption>Dettagli della notifica Webhook</caption>
  <tr>
     <th>Campo</th>
     <th>Descrizione</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Un identificativo univoco della notifica. Questo campo è obbligatorio.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Seleziona **Webhook**</td>
  </tr>
  <tr>
    <td>Webhook URL</td>
    <td>Immetti l'URL dove deve essere eseguito il POST.</td>
  </tr>
  <tr>
  <td>Verify certificates</td>
    <td>Seleziona per verificare i certificati.</td>
  </tr>
  <tr>
    <td>Webhook headers</td>
    <td>Immetti le eventuali intestazioni.</td>
  </tr>
  <tr>
    <td>Webhook query parameters</td>
    <td>Immetti gli eventuali parametri query.</td>
  </tr>
</table>

<table>
  <caption>Dettagli di notifica di pager duty</caption>
  <tr>
     <th>Campo</th>
     <th>Descrizione</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Un identificativo univoco della notifica. Questo campo è obbligatorio.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Seleziona **Pager duty**</td>
  </tr>
  <tr>
    <td>API Key</td>
    <td>Immetti la chiave API per le notifiche pager duty.</td>
  </tr>
</table>


5. Fai clic su **Ok** per creare le nuove notifiche con l'impostazione che hai specificato.

## Modifica una notifica
 1. Dopo che hai aderito al programma beta, seleziona **Devices -> Monitoring**. 
 2. Fai clic sulla scheda **Notifications**.
3. Fai clic su **Actions->Edit Notification**.
4. Modifica qualsiasi dettaglio di notifica.
5. Fai clic su **Ok** per accettare le tue modifiche.

## Elimina una notifica
1. Dopo che hai aderito al programma beta, seleziona **Devices -> Monitoring**. 
2. Fai clic sulla scheda **Notifications**.
3. Fai clic su **Actions->Delete Notification**.
4. Fai clic su **Delete** per confermare la tua scelta.

## Aggiungi più notifiche a un dispositivo
1. Seleziona **Infrastructure->Device List->*Device Name*** per accedere ai dettagli del dispositivo.
2. Fai clic su **Actions->Manage notifications**.
4. Fai clic per assegnare o rimuovere notifiche per il tuo dispositivo.

