---

copyright:
  years: 2014, 2017
lastupdated: "2017-10-30"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configurazione di un report agent del monitoraggio Nimsoft

1. Dalla schermata di monitoraggio, seleziona **Configure Agent Reports** dal menu a discesa **Actions** nella colonna **Advanced**.

2. Seleziona l'agent da configurare dall'elenco a discesa **Agents**.
  * **Nota:** gli agent disponibili variano in base al dispositivo e dipendono dal pacchetto di monitoraggio applicato al dispositivo.

3. Seleziona la sezione da configurare dall'elenco a discesa **Sections**. Se selezioni una sezione che contiene dei profili, viene visualizzato un altro elenco a discesa. Da tale elenco, seleziona un **profilo esistente** dall'elenco a discesa **Profiles**. Per aggiungere una nuova configurazione, seleziona **Add Agent Config...** dall'elenco a discesa **Profiles**.

4. Completa ciascun campo nella sezione **General metrics and information**, se necessario.
  * **Nota:** i campi obbligatori sono indicati da un asterisco rosso (*). Non tutti gli agent, sezioni o profili contengono questa sezione.

5. Fai clic sulla casella di spunta **Metric** per ciascuna metrica da includere nel report dalla sezione **Select metrics to report on**, se applicabile.

6. Fai clic sulla casella di spunta **Alarm** per ciascun avviso da attivare per l'agent da **Metric Alarms**.
  * **Nota:** non tutti gli avvisi in questa sezione sono collegati a una specifica metrica. Gli avvisi vengono inviati a ogni indirizzo email associato alla sezione **Alarm Subscribers** per l'agent.

7. Fai clic su **Save** per salvare la configurazione. Fai clic su **Cancel** per annullare l'azione.
  * **Nota:** il pulsante di salvataggio è disabilitato finché non apporti una modifica alla configurazione attuale.

## Passi successivi

Dopo che hai correttamente salvato la configurazione, viene visualizzato un messaggio di conferma. Se la configurazione non è riuscita, viene visualizzato un messaggio di errore con i dettagli sull'errore che si è verificato e come correggerlo. Puoi riconfigurare gli agent in qualsiasi momento ripetendo questa procedura.
