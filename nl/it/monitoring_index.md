---

copyright:
  years: 2014, 2018
lastupdated: "2018-11-15"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Monitoraggio
{{site.data.keyword.BluSoftlayer_full}} offre i servizi di monitoraggio standard e il monitoraggio Nimsoft per garantirti di essere sempre al corrente di eventuali problemi con i tuoi dispositivi. I servizi di monitoraggio standard includono funzioni come Ping e Monitoraggio NOC. Il monitoraggio Nimsoft comprende tre livelli di monitoraggio, che includono il monitoraggio di base, avanzato e premium. Ogni servizio in entrambe le offerte di monitoraggio standard e Nimsoft offre diversi vantaggi; sono disponibili a diverse opzioni di prezzo per soddisfare le tue esigenze di business. Per ulteriori informazioni, consulta [{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}.

Il monitoraggio di un dispositivo consente agli utenti di avviare i ping lenti e del servizio per assicurarsi che il dispositivo sia online e reattivo.

Se non viene ricevuta una risposta echo nell'intervallo di tempo assegnato (1 secondo per i ping del servizio, 5 secondi per i ping lenti)
viene inviato un avviso all'indirizzo email nell'account. Uno stato di **Up** nel campo **Status** indica
che è stata ricevuta una risposta echo, mentre **Down** indica che la risposta echo non è stata ricevuta. 

Per visualizzare i monitoraggi configurati, attieniti alla seguente procedura:

1. Dal Device List, fai clic sul nome dispositivo (**Device Name**) per accedere al dispositivo.

2. Fai clic sulla scheda **Monitoring**. Tutti i ping correnti sono visualizzabili nella pagina di destinazione. (La scheda **Monitoring** è visibile solo se è configurato almeno un monitoraggio).
