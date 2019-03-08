---

copyright:
  years: 2014, 2018
lastupdated: "2018-10-30"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Modifica di un monitoraggio esistente
Dopo che un monitoraggio è stato aggiunto a un dispositivo, puoi modificarlo o rimuoverlo in qualsiasi momento. Le modifiche ai monitoraggi consentono di apportare modifiche alle opzioni di tipo e notifica, mentre la rimozione di un monitoraggio annulla completamente il monitoraggio. Attieniti alla seguente procedura per modificare un monitoraggio esistente:

1. Nella pagina **Monitors** sotto l'intestazione **Edit Existing Monitors**, fai clic su uno qualsiasi dei dettagli del monitoraggio per aprire il monitoraggio per le modifiche.

2. Modifica i dettagli del monitoraggio (**Monitor Details**) come necessario. Fai riferimento a questa tabella per ulteriori dettagli su ciascun campo modificabile. 

|Campo|Dettagli|Azione|
|---|---|---|
|Monitor Type|Il lasso di tempo entro cui è prevista una risposta dal dispositivo. Il sistema ha come valore predefinito un ping del servizio. Un ping lento attende una risposta per 5 secondi, consentendo ai server ottimizzati per le attività non di rete più tempo per elaborare la richiesta. Un ping del servizio emette un ping ogni 5 minuti e attende una risposta echo entro 1 secondo. Se viene mancato più di un ping, viene generato un avviso.|Seleziona da **Slow Ping** o **Service Ping**.|
|Notify| Gli utenti notificati ricevono delle notifiche automatizzate ogni volta che un dispositivo non risponde a un ping entro il tempo di risposta allocato. Per la notifica, un utente deve trovarsi nell'account associato al dispositivo per ricevere una notifica. |Per aggiungere un utente, seleziona il nuovo utente notificato (**Notified User**) e fai clic su **Add User**. Per rimuovere un utente, fai clic sull'icona **Remove** accanto all'utente notificato (Notified User) esistente e fai clic su **Yes** per confermare la tua azione.|
|Notify Wait|Il lasso di tempo per cui il sistema attende prima di inviare una notifica nel caso in cui il dispositivo non abbia risposto al ping. Sono disponibili molteplici tempi di attesa. **Nota:** i dettagli della notifica non sono necessari quando non è selezionato alcun utente per la notifica. |Seleziona il tempo di attesa di cui hai bisogno.|

3. Fai clic su **Update** per applicare le modifiche al monitoraggio. Fai clic su **Cancel** per annullare l'azione.

## Passi successivi

Se viene modificato, un monitoraggio continua a funzionare come specificato nei dettagli del monitoraggio. Se viene modificato il tipo, la quantità di tempo per ricevere il ping previsto è differente. Se le opzioni di notifica subiscono delle modifiche, la modalità di notifica viene modificata in base alle nuove selezioni. Il monitoraggio rimane accessibile dalla scheda Monitoring.
