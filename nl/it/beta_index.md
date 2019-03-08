---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# Introduzione a IBM Cloud Monitoring (Beta)
{: #gettingstartedbeta}

Questa applicazione di monitoraggio beta, sviluppata sul {{site.data.keyword.BluSoftlayer_full}} Monitoring Service, è disponibile per i server virtuali e bare metal. Per aggiornamenti sullo sviluppo di questo programma Beta, consulta il [blog di IBM Cloud![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}.
{:shortdesc}

## Prerequisiti

Per partecipare a questo programma Beta, devi soddisfare i seguenti requisiti:
1. Il tuo account SoftLayer deve essere collegato a un account IBM Cloud con l'autenticazione ID IBM. Per collegare un account, l'utente master sul tuo account SoftLayer deve eseguire l'accesso al [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com){: new_window} e dal menu **Account**, devi fare clic su **Link a Bluemix Account!**.
2. Per visualizzare il programma Beta, ogni utente deve essere collegato a un ID IBM. Per ulteriori informazioni, consulta [Collegamento degli account utente ID IBM](/docs/account?topic=account-unifyingaccounts#link_customer_accounts).
3. Per visualizzare il programma Beta, ogni utente deve disporre dell'accesso a IBM Cloud Monitoring Service.
   1. Dalla [console IBM Cloud ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://console.bluemix.net){: new_window}, seleziona **Manage -> Account -> Users**.
   2. Invita l'utente all'account oppure seleziona l'utente dall'elenco.
   3. Seleziona **Assegna l'accesso alle risorse** per l'utente.
   4. Da **Servizio**, seleziona **IBM Cloud Monitoring Service**.
   5. Seleziona il **Ruolo** da concedere all'utente per tutte le regioni.

Se non soddisfi questi prerequisiti, non puoi accedere al monitoraggio Beta, al momento.


## Adesione al programma Beta

Attieniti alla seguente procedura per un'introduzione al programma Beta di monitoraggio. Aderire al programma Beta abilita il servizio per tutti i server virtuali e bare metal idonei nel tuo account. Fare clic sull'opzione di adesione non influenza i dati o il monitoraggio Nimsoft esistenti.
1. (Solo bare metal) [Installa l'agent di monitoraggio sul tuo server bare metal](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-).
<table>
   <CAPTION>Tabella 1. Scegli un'ubicazione di accesso</CAPTION>
   <THEAD>
   <TR>
   <th>Se vuoi aderire con...</th>
   <th>Allora...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Catalogo IBM Cloud</td>
   <td>
   <ol>
   <li>Apri una nuova finestra del browser e immetti <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>.</li>
   <li>Fai clic sul link <b>Accedi</b>. </li>
   <li>Immetti la tua email o il tuo id IBM e fai clic su <b>Continua.</b></li>
   <li>Immetti la tua password e fai clic su <b>Accedi</b></li>
   <li>Seleziona **Infrastructure->Device List->*Device Name*** per accedere ai dettagli del dispositivo.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Portale dei clienti</td>
   <td>
   <ol>
   <li>Apri una nuova finestra del browser e immetti <a href="https://control.softlayer.com">https://control.softlayer.com</a>.</li>
   <li>Immetti il tuo nome utente e la tua password e fai clic su <b>Accedi</b>. In alternativa, fai clic su <b>Accedi con id IBM</b>. Immetti quindi la tua email o il tuo id IBM e fai clic su <b>Continua</b>. Immetti la tua password e fai clic su <b>Accedi</b>. Viene aperta la pagina principale del {{site.data.keyword.slportal}}.</li>
     <li>Da **Devices**, fai clic sul nome dispositivo (**Device Name**) per accedere ai dettagli del dispositivo.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. Seleziona **Devices -> Monitoring**. Fai clic su **Join the beta** per visualizzare le schede beta delle notifiche e delle politiche di sistema.

## Passi successivi
1. Riesamina i dettagli delle [metriche](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-) raccolte.
2. [Crea o gestisci](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-) una notifica di monitoraggio.
3. [Crea o gestisci](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-) una politica di sistema.
4. [Visualizza gli avvisi](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-).
5. Riesamina i dati del grafico di monitoraggio Beta attualmente disponibili per un dispositivo selezionato.

|              Metriche                                      |  Descrizione                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU utilization                                            |   Visualizza l'utilizzo percentuale (% ) della CPU per ogni core e una media sui core. Fai clic su ciascuna metrica nella chiave per attivare o disattivare i dati sul grafico.
|Public network                                             |   Visualizza i dati in entrata e in uscita per la tua rete pubblica. Fai clic su ciascuna metrica nella chiave per attivare o disattivare i dati sul grafico.       |
|Private network                                            |   Visualizza i dati in entrata e in uscita per la tua rete privata. Fai clic su ciascuna metrica nella chiave per attivare o disattivare i dati sul grafico.           |
|Memory utilization    | Visualizza l'utilizzo percentuale (% ) di memoria per il tuo server     |
|Disk usage    | Visualizza la quantità media di dati letta o scritta dal o sul disco in byte oppure la latenza del disco. Fai clic su ciascuna metrica nella chiave per attivare o disattivare i dati sul grafico.    |
|Temperature                                                 |Visualizza la temperatura del tuo dispositivo bare metal in gradi Celsius. Questi dati non sono disponibili per tutti i dispositivi.
{: caption="Tabella 1. Metriche beta" caption-side="top"}   

## Limitazioni
Se un dispositivo viene eliminato, le politiche di monitoraggio associati non vengono eliminate. Tieni presente che devi eliminare manualmente il dispositivo per queste politiche.

I dati delle metriche sono disponibili solo per 15 giorni.

Possono esistere solo 10 politiche di monitoraggio contemporaneamente. Tuttavia, una politica può essere applicata a più dispositivi.

## risoluzione dei problemi
Per visualizzare alcune metriche, come l'utilizzo della memoria, sono necessari degli strumenti Xen sul tuo server. Per informazioni sull'installazione degli strumenti Xen, consulta la pagina relativa alla [preparazione e importazione di immagini](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images).

## Feedback
Per fornire un feedback su questo programma Beta, seleziona **Devices -> Monitoring** oppure la pagina dei dettagli del dispositivo e fai clic su **Leave feedback** per completare un breve sondaggio. Per uscire dal programma Beta e ritornare alla vista standard, fai clic sul link **Leave the Beta** alla fine della pagina **Devices -> Monitoring**.
