Un amministratore può ottenere una vista olistica dell'integrità attuale e passata del dispositivo in un solo posto.

Rapporti utente:

    Qualsiasi utente può rapidamente alternare le schede "Bandwidth" e "Usage" tra la loro vista esistente e la versione beta di Observer (solo BETA)

    Qualsiasi utente può fornire un feedback sulla sua esperienza nella versione beta di Observer tramite il portale di controllo (solo BETA)

    Qualsiasi utente può accedere al post del blog per ulteriori informazioni sul nostro lavoro su Observer nell'esperienza beta (solo BETA)

    Gli utenti hanno un posto designato dove possono archiviare e visualizzare le metriche delle risorse dell'infrastruttura per i server virtuali:

    1. CPU utilization, %, per virtual core

    2. Network-Public, in/out, bytes and packets

    3. Network- Private, in/out, bytes and packets

    4. Memory utilization, %

    5. Disk Read, bytes and ops

    6. Disk Write, bytes and ops

    7. Transmit errors, in/out, count

    8. Disk Latency, ms, read and write

    9. Local disk utilization, % and bytes used and total bytes available


    Gli utenti bare metal potranno visualizzare le seguenti metriche:

    1. CPU utilization, %, per virtual core

    2. Network-Public, in/out, bytes and packets

    3. Network- Private, in/out, bytes and packets

    4. Memory utilization, %

    5. Disk Read, bytes and ops

    6. Disk Write, bytes and ops

    7. Transmit errors, in/out, count

    8. Disk Latency, ms, read and write

    9. Local disk utilization, % and bytes used and total bytes available

    10. RAID Alerts, 0/1

    11. Core temperature, degrees F

    Tutti gli amministratori possono visualizzare la cronologia di avvisi e metriche in una singola vista senza dovere eseguire alcuna analisi delle registrazioni nei log. (Analogo a #60)

    Un gestore può comprendere lo stato di integrità generale del suo dispositivo senza aver bisogno di chiarimenti dai suoi team di amministrazione.

    Qualsiasi utente può aprire il file syslog più recente di un dispositivo senza utilizzare la riga di comando (simile a #35)

    Qualsiasi utente può visualizzare ed esplorare in qualsiasi momento i dati delle metriche di qualsiasi serie temporale in una serie di grafici interattivi.

    Qualsiasi utente può visualizzare e comprendere gli elementi basilari della cronologia degli avvisi.

    Qualsiasi utente può contrassegnare gli eventi come "aperti" o "chiusi".

    Nessun utente ha bisogno di creare manualmente un evento ogni qual volta viene attivato un avviso.

    Nessun utente ha bisogno di assegnare manualmente un livello di severità di "avvertenza" o "errore", ad eccezion fatta per le loro impostazioni degli avvisi.

    Qualsiasi utente può raccogliere metriche a livello di sistema e applicazione utilizzando gli agent collectID per risposte URL, MySQL, MSSQL, tomcat, apache e processi di monitoraggio.

    Un amministratore può inviare dei dati di metriche personalizzate nel servizio di monitoraggio in un modo automatizzato.

    Qualsiasi utente può utilizzare metriche di sistema, applicazione o personalizzate nello stesso modo delle metriche hypervisor: grafici, dashboard, avvisi, notifiche, risposte automatiche, template ecc.



Hill 2: un amministratore può comprendere e iniziare a risolvere un incidente entro 90 secondi.

Rapporti utente:

    Qualsiasi amministratore può sottoscrivere avvisi senza essere inondato di falsi positivi.

    Qualsiasi amministratore può ricevere avvisi tramite il suo canale di comunicazione di elezione entro un minuto dal verificarsi di un evento di trigger.

    Gli ingegneri responsabili dell'affidabilità possono comprendere la causa di un avviso di incidente sulla base del messaggio nell'avviso stesso.

    Qualsiasi amministratore può controllare le metriche di utilizzo recenti su qualsiasi dispositivo con un elevato grado di accuratezza.

    Qualsiasi amministratore può cercare le esatte informazioni di cui ha bisogno in meno di 10 secondi.

    Un non amministratore può risolvere un incidente per cui è stata eseguita una escalation con meno di tre messaggi dal supporto SL.

    Qualsiasi utente può specificare una condizione per una segnalazione di qualsiasi metrica disponibile (predefinita, collectD o personalizzata).

    Qualsiasi utente può specificare una condizione basata su un valore medio, un valore cumulativo (somma), un valore minimo o un valore massimo di qualsiasi metrica.

    Qualsiasi utente può specificare una condizione con la qualifica "maggiore di" o "minore di".

    Qualsiasi utente può specificare il numero di periodi consecutivi per cui una condizione deve essere soddisfatta, nonché la lunghezza del periodo (30 secondi o 5 minuti) prima che venga attivato un avviso - "se X si verifica per 2 periodi consecutivi di 30 secondi, l'avviso viene attivato"

    Qualsiasi utente può specificare più condizioni per un singolo avviso "se questo E questo E questo, allora l'avviso viene attivato".

    Qualsiasi utente può specificare un nome personalizzato per l'avviso.

    Qualsiasi utente può essere informato di avvisi che indicano l'ora, il nome dell'avviso e le condizioni soddisfatte che hanno attivato l'avviso.

    Nessun utente, dopo che un avviso è stato attivato, riceverà avvisi aggiuntivi dalla stessa regola sullo stesso dispositivo finché l'avviso iniziale non sarà stato "chiuso".

    Regola di avviso di esempio: se la media di utilizzo della CPU è superiore all'80% per 2 periodi consecutivi di 5 minuti E la somma di traffico in entrata della rete è superiore ai 50 GB per 1 periodo consecutivo di 5 minuti, viene attivato un avviso e viene creato un evento (presumendo che gli eventuali avvisi precedenti per questa regola siano stati chiusi).

    Un amministratore può specificare 1 o più indirizzi email per notificare qualsiasi utente.

    Un amministratore può specificare 1 o più numeri di telefono per SMS per notificare qualsiasi utente.

    Un amministratore può specificare 1 o più URL per i webhook da inviare.

    Un amministratore può specificare il gruppo Pagerduty per notificare gli utenti.

    Un amministratore può specificare se il server deve eseguire il riavvio o l'arresto quando viene attivato l'avviso.

    Un amministratore può specificare un intervallo di 30 secondi o 5 minuti per il monitoraggio rete di qualsiasi protocollo supportato

    Un amministratore può implementare i controlli ping dell'host (ICMP)

    Un amministratore può implementare i controlli delle porte TCP per diversi protocolli DNS, DNS personalizzato, FTP, HTTP, HTTP personalizzato, HTTPS, IMAP, LDAP, NNTP, POP, SMTP, SSH, TCP personalizzato, TELNET, UDP SIP (il supporto per questi protocolli è presente nell'attuale offerta SL TCP).

    Un amministratore può implementare un controllo della porta TCP per il protocollo SNMP (non attualmente supportato nell'offerta SL esistente)

    Un amministratore può specificare la soglia per il tempo di risposta per essere riconosciuta come operazione riuscita oppure errore.

    Un amministratore può specificare il numero di errori consecutivi da un ping dell'host o un controllo della porta TCP prima che venga attivato un avviso.

    Un amministratore può implementare le stesse opzioni di notifica e risposta automatizzata dagli avvisi di monitoraggio di rete degli avvisi basati sulle metriche (email, SMS, webhook, PagerDuty, riavvio, arresto).

    Un amministratore può specificare il livello di severità di "avvertenza" o di "errore" sia per gli avvisi di monitoraggio di rete che per quelli di metrica.



Hill 3: qualsiasi utente può configurare il monitoraggio su qualsiasi dispositivo, dedicando meno di 90 secondi alle decisioni relative alla configurazione. (Analogo a #59)

Rapporti utente:

    Un non amministratore può in pratica configurare il suo monitoraggio utilizzando solo l'interfaccia e la documentazione.

    Un amministratore può configurare un monitoraggio che soddisfi le sue specifiche esigenze selezionando configurazioni salvate o preconfezionate senza dover affrontare il processo di configurazione manuale. (Analogo a #58)

    Un amministratore può configurare un monitoraggio che soddisfi le sue esigenze specifiche modificando e salvando manualmente una configurazione e applicarlo a qualsiasi numero di dispositivi.

    Un amministratore può configurare gli avvisi su più dispositivi con il minimo sforzo ripetitivo.

    Qualsiasi utente può esportare dati specifici per le metriche e per il tempo in un file CSV.

    Un amministratore o un gestore può configurare una finestra di manutenzione durante la quale non verrà inviata alcuna notifica quando vengono attivati degli avvisi.

    Qualsiasi utente stabilito può comprendere e applicare le configurazioni salvate. (Analogo a #41)

    Qualsiasi nuovo utente può comprendere e applicare configurazioni preconfezionate. (Analogo a #34, #32)

    Un non amministratore può ottenere supporto per la configurazione del monitoraggio senza compilare un ticket di supporto.

    Ogni cliente può ordinare il monitoraggio per qualsiasi dispositivo senza competenze specialistiche. (Analogo a #63, #43)

    Tutti i clienti hanno un'esperienza unificata e prevedibile per l'ordinazione del monitoraggio per qualsiasi dispositivo. (Analogo a #40)

    Qualsiasi utente può integrare il suo dispositivo con un servizio di terze parti senza compilare un ticket di supporto.

    Nessun utente ha bisogno di creare manualmente un avviso per gli avvisi di "avvertenza" relativi al ciclo di vista: creazione, avvio, arresto.

    Qualsiasi utente tecnico può accedere a tutta la funzionalità Observer tramite la stessa API come il resto del servizio di monitoraggio.

    IBM può limitare l'accesso degli account ab a specifiche funzioni/prestazioni con la versione gratuita, come definito nella panoramica di Observer per la messa a confronto tra il livello gratuito e quello a pagamento.

    Qualsiasi cliente può eseguire l'upgrade da una versione gratuita a una a pagamento all'interno della scheda Monitoring.

    Qualsiasi cliente può eseguire un upgrade oppure un downgrade da una versione a pagamento a una gratuita nell'area di gestione degli account.

    Qualsiasi utente con la versione gratuita può visualizzare le opzioni di cui disporrebbe se avesse eseguito un upgrade ma in un modo tale che indica perché non sono disponibili.

    Se un utente prova ad eseguire un'azione che richiederebbe un upgrade, dovrebbe vedere un messaggio che spiega che deve eseguire un upgrade e che offre un'alternativa, se ne esiste una (ad esempio il messaggio indica all'utente che già ha il numero massimo di avvisi per la versione gratuita e lo invita quindi ad eseguire un upgrade oppure ad eliminare un avviso per creare una nuova regola).


