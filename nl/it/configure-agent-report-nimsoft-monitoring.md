---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configurazione di un report agent del monitoraggio Nimsoft
{: #configuring-a-nimsoft-monitoring-agent-report}

## Prima di cominciare

Per prima cosa passa al menu del dispositivo e assicurati di disporre delle autorizzazioni account corrette per completare le attività.

* Passa al menu del dispositivo della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assicurati di avere tutte le autorizzazioni account necessarie e l'accesso al dispositivo. Solo il proprietario dell'account o un utente con l'autorizzazione dell'infrastruttura classica **Manage Users**, può modificare le autorizzazioni.

Per ulteriori informazioni sulle autorizzazioni, vedi [Autorizzazioni dell'infrastruttura classica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gestione accesso dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Configurazione di un report agent del monitoraggio Nimsoft
{: #configuring-nimsoft-monitoring-agent-report-steps}

Completa la seguente procedura per configurare un report agent del monitoraggio Nimsoft.

1. Dal menu **Devices**, seleziona **Monitoring**.
2. Dalla pagina **Monitoring**, seleziona **Configure Agent Reports** dal menu a discesa **Actions** nella colonna **Advanced**.
3. Seleziona l'agent da configurare dall'elenco a discesa **Agents**.
  
  Gli agent disponibili variano in base al dispositivo e dipendono dal pacchetto di monitoraggio applicato al dispositivo.
  {:note}

4. Seleziona la sezione da configurare dall'elenco a discesa **Sections**. Se selezioni una sezione che contiene dei profili, viene visualizzato un altro elenco a discesa. Da tale elenco, seleziona un **profilo esistente** dall'elenco a discesa **Profiles**. Per aggiungere una nuova configurazione, seleziona **Add Agent Config...** dall'elenco a discesa **Profiles**.

5. Completa ciascun campo nella sezione **General metrics and information**, se necessario.
  
  I campi obbligatori sono indicati con un asterisco rosso (*). Non tutti gli agent, sezioni o profili contengono questa sezione.
  {:note}

6. Fai clic sulla casella di spunta **Metric** per ciascuna metrica da includere nel report dalla sezione **Select metrics to report on**, se applicabile.

7. Fai clic sulla casella di spunta **Alarm** per ciascun avviso da attivare per l'agent da **Metric Alarms**.

  Non tutti gli avvisi in questa sezione sono collegati a una specifica metrica. Gli avvisi vengono inviati a ogni indirizzo email associato alla sezione **Alarm Subscribers** per l'agent.
  {:note}

7. Fai clic su **Save** per salvare la configurazione. Fai clic su **Cancel** per annullare l'azione.
  
  Il pulsante **Save** è disabilitato finché non apporti una modifica alla configurazione attuale.
  {:note}

## Passi successivi

Dopo che hai correttamente salvato la configurazione, viene visualizzato un messaggio di conferma. Se la configurazione non è riuscita, viene visualizzato un messaggio di errore con i dettagli sull'errore che si è verificato e come correggerlo. Puoi riconfigurare gli agent in qualsiasi momento ripetendo questa procedura.
