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

# Visualizzazione di un report agent per il monitoraggio Nimsoft
{: #viewing-an-agent-report-for-nimsoft-monitoring}

I dettagli del monitoraggio per il monitoraggio Nimsoft sono disponibili nei report agent, che forniscono i dettagli specifici per il modo in cui l'agent è stato configurato. 
{:shortdesc}

## Prima di cominciare
Per prima cosa passa al menu del dispositivo e assicurati di disporre delle autorizzazioni account corrette per completare le attività.

* Passa al menu del dispositivo della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assicurati di avere tutte le autorizzazioni account necessarie e l'accesso al dispositivo. Solo il proprietario dell'account o un utente con l'autorizzazione dell'infrastruttura classica **Manage Users**, può modificare le autorizzazioni.

Per ulteriori informazioni sulle autorizzazioni, vedi [Autorizzazioni dell'infrastruttura classica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gestione accesso dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Visualizzazione di un report agent per il monitoraggio Nimsoft
{: #viewing-agent-report-nimsoft-monitoring-steps}

Completa la seguente procedura per visualizzare un report agent per il monitoraggio Nimsoft.

1. Dalla pagina **Monitoring**, seleziona **View Agent Reports** dal menu **Actions**.
2. Seleziona l'agent da visualizzare dall'elenco **Agents**.

  Gli agent disponibili variano in base al dispositivo e dipendono dal pacchetto di monitoraggio applicato al dispositivo.
  {:note}
  
3. Completa tutte le sezioni restanti, includendo una o più delle seguenti azioni:

  Ogni agent varia e non include ogni sezione o metrica. Le opzioni disponibili in questa schermata dipendono dalle opzioni di configurazione disponibili per ogni agent.
  {:note}
  
  * Seleziona la sezione report dall'elenco **Sections**.
  * Seleziona il periodo di tempo per il report dall'elenco **View By**.
  * Fai clic sulla casella di spunta per ciascuna metrica che vuoi includere nel report nella sezione **Select metrics to report on:**.
    
    Vengono visualizzate solo metriche simili nello stesso grafico. Se vengono scelte delle metriche in conflitto, si verificherà un errore dopo che avrai richiesto il grafico.
    {:note}
4. Fai clic su **Draw Graph** per tracciare il grafico.

## Passi successivi

Dopo che il grafico per il report agent è stato tracciato, è possibile tracciarlo nuovamente in qualsiasi momento per visualizzare delle metriche differenti ripetendo la procedura indicata. Non c'è alcun limite al numero di report agent che possono essere generati entro uno specifico lasso di tempo.
