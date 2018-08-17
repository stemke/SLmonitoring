---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# Domande frequenti sul monitoraggio

<a name="48"></a>
## Vedo numerosi ticket di avviso del monitoraggio. Questo significa che il mio server è inattivo?

Ogni dispositivo è dotato di un servizio di notifica e ping di monitoraggio gratuito. Questo servizio crea automaticamente un ticket di avviso di monitoraggio in caso di errore con specifici parametri. Dei falsi positivi sono possibili con il servizio di monitoraggio e possono essere attribuiti alla limitazione della velocità a opera di un firewall software sul server, alla disponibilità di servizi e applicazioni e elle interruzioni dei servizi all'interno dell'infrastruttura di monitoraggio. Riesamina le impostazioni predefinite per ridurre i possibili falsi avvisi di monitoraggio. 

<a name="354"></a>
## Posso fare in modo che il sistema di monitoraggio esegua un riavvio automatico e avvisi un tecnico di supporto se il server smette di rispondere?

Sì, con il servizio **Automated Reboot from Monitoring Failure** puoi configurare il sistema automatico in modo che esegua automaticamente il riavvio del server ed emetta un ticket per il tecnico di supporto se viene generato un avviso di monitoraggio. 

<a name="1699"></a>
## Qual è la differenza tra il monitoraggio con un “ping lento”) e un “ping del servizio”?

La differenza tra un ping del servizio e un ping lento consiste nel lasso di tempo entro cui è prevista una risposta da un dispositivo. Il valore predefinito è il ping del servizio ma è possibile apportare una modifica per utilizzare invece un ping lento.

* Un ping del **servizio** emette un ping ogni 5 minuti e attende una risposta echo entro 1 secondo. Se viene mancato più di un ping, viene generato un avviso.
* Un ping **lento** attende una risposta per 5 secondi, consentendo ai server ottimizzati per le attività non di rete più tempo per elaborare la richiesta.


<a name="1000"></a>
## Quando viene aperto un ticket di monitoraggio che mi avvisa del problema, i tecnici vedranno il ticket e risponderanno?

Con il servizio ping di base, i tecnici di supporto non ricevono notifiche degli errori. Questi ticket vengono aperti quando il sistema di monitoraggio genera un avviso e informano solo gli utenti da te specificati nella schermata di monitoraggio, I tecnici non vengono informati finché non apri un nuovo ticket indicando che il server non sta rispondendo.

