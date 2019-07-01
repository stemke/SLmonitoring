---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Esercitazione introduttiva 
{: #monitoring}

{{site.data.keyword.cloud}} offre i servizi di monitoraggio standard e il monitoraggio Nimsoft per garantirti di essere sempre al corrente di eventuali problemi con i tuoi dispositivi. I servizi di monitoraggio standard includono funzioni come Ping e Statistiche IPMI. Il monitoraggio Nimsoft comprende tre livelli di monitoraggio, che includono il monitoraggio di base, avanzato e premium. Ogni servizio in entrambe le offerte di monitoraggio standard e Nimsoft offre diversi vantaggi; sono disponibili a diverse opzioni di prezzo per soddisfare le tue esigenze di business. Per ulteriori informazioni, consulta [{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}.
{:shortdesc}

Il monitoraggio di un dispositivo ti consente di avviare i ping lenti e del servizio per assicurarsi che il dispositivo sia online e reattivo.

Se non viene ricevuta una risposta echo nell'intervallo di tempo assegnato (1 secondo per i ping del servizio, 5 secondi per i ping lenti)
viene inviato un avviso all'indirizzo email nell'account. Uno stato di **Up** nel campo **Status** indica
che è stata ricevuta una risposta echo, mentre **Down** indica che la risposta echo non è stata ricevuta.

Per visualizzare i monitoraggi configurati, attieniti alla seguente procedura:

1. Passa al menu del dispositivo della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
2. Dal menu **Devices**, seleziona **Device List** e seleziona il dispositivo.
3. Fai clic sulla scheda **Monitoring**. Tutti i ping correnti sono visualizzabili nella pagina di destinazione. 

La scheda **Monitoring** è visibile solo se è configurato almeno un monitoraggio.
{:note}

