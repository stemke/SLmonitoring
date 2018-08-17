---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Scansioni delle vulnerabilità
{{site.data.keyword.BluSoftlayer_full}} collabora con Nessus per fornire scansioni delle vulnerabilità per qualsiasi dispositivo nella rete {{site.data.keyword.BluSoftlayer_notm}}.  Le scansioni delle vulnerabilità testano le aree di debolezza in un dispositivo e restituiscono un report dell'analisi, dei problemi di sicurezza e delle correzioni per il tuo dispositivo host. L'esecuzione delle scansioni delle vulnerabilità sui tuoi dispositivi garantisce che rimangano sempre protetti e sono anche la prima risorsa da utilizzare quando pensi che un dispositivo potrebbe essere vulnerabile o compromesso. Le scansioni delle vulnerabilità vengono completate utilizzando il [Portale dei clienti ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/) su qualsiasi dispositivo associato al tuo account.
{:shortdesc}

## Scanner della sicurezza Nessus 
{{site.data.keyword.BluSoftlayer_notm}} fornisce uno scanner della sicurezza online, che si avvale della tecnologia dello strumento open source di scansione Nessus. È possibile accedere a questo scanner della sicurezza nella scheda Security facendo clic su **Scanner**. Per ulteriori informazioni, consulta la pagina relativa allo [strumento di scansione Nessus ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://www.nessus.org/nessus/).

La pagina **Scanner** fornisce un elenco dell'hardware disponibile per lo strumento Nessus ospitato da {{site.data.keyword.BluSoftlayer_notm}}. Per eseguire la scansione di un server, o per visualizzare i risultati di una scansione precedente, fai clic sul link dei dettagli per il server che desideri ispezionare. La pagina dei dettagli della scansione delle vulnerabilità mostra un breve riepilogo del server (contenente il nome del server, l'indirizzo IP di cui eseguire la scansione e il data center dove si trova il server). **Start Scan** pianifica il tuo server presso il server di scansione Nessus perché ne venga eseguita la scansione delle vulnerabilità appena possibile.

Dopo il riepilogo del server è presente una tabella delle scansioni delle vulnerabilità di Nessus attuali e passate. Per ogni scansione è elencata la data in cui la scansione era stata richiesta, la data in cui la scansione era stata avviata, lo stato della scansione e, nel caso in cui la scansione sia stata completata, un link al report Nessus.

I report Nessus possono avere uno dei seguenti stati:

* Scan Pending: la scansione è stata pianificata per il box dello scanner di Nessus.
* Scan Processing: la scansione è attualmente in corso.
* Generating Report: la scansione è stata completata ed è in corso la compilazione dei risultati del test in un report.
* Scan Complete: la scansione è stata completata correttamente e il report delle vulnerabilità è stato generato.
* Scan Cancelled: la scansione Nessus è stata annullata manualmente da un tecnico di {{site.data.keyword.BluSoftlayer_notm}}.

Per tutte le scansioni Nessus completate correttamente che sono elencate in questa tabella, è possibile visualizzare un report facendo clic su **View Report**. Il report presenta due tabelle: una tabella Scan Details, che elenca il numero di host di cui è stata eseguita la scansione, il numero di vulnerabilità della sicurezza aperte (falle) rilevati e il numero di possibili vulnerabilità della sicurezza (avvertenze) trovato. La seconda tabella elenca tutti i problemi di sicurezza rilevati: l'host su cui è stata rilevata la vulnerabilità e una descrizione della possibile vulnerabilità.

Lo strumento Nessus open source è basato sui plug-in, il che consente di sviluppare dei nuovi test man mano che vengono rilevate delle vulnerabilità. {{site.data.keyword.BluSoftlayer_notm}} aggiorna lo strumento Nessus interno regolarmente; si consiglia pertanto di eseguire regolarmente delle scansioni con lo scanner di sicurezza per tenersi al passo con le nuove minacce.

Perché la scansione riesca, è necessario consentire l'accesso al tuo server sia da 173.192.255.232 che da 172.17.19.38.
