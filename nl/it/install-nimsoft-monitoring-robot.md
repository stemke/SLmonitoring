---

copyright:
  years: 2014, 2019
lastupdated: "2019-02-11"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installazione e gestione del Nimsoft Monitoring Robot
{: #installing-and-managing-the-nimsoft-monitoring-robot}

Per consentire il funzionamento del monitoraggio avanzato su {{site.data.keyword.baremetal_short}} o su {{site.data.keyword.BluVirtServers_short}} esistenti, installa il Nimsoft Monitoring Robot. Il Nimsoft Monitoring Robot consente al sistema di gestione del monitoraggio di comunicare con il server bare metal o il server virtuale sulla rete privata. Dopo che hai installato il Nimsoft Monitoring Robot, ci vogliano circa 5 - 10 minuti perché diventi disponibile nel {{site.data.keyword.slportal_full}}. Attieniti alla seguente procedura per installare il Nimsoft Monitoring Robot in Windows o Linux.

## Prerequisiti

Prima di eseguire l'installazione, le seguenti porte devono essere aperte sulla rete privata:

* tcp/48000
* tcp/48001
* tcp/48002

Apri inoltre le porte da tcp/48003 a tcp/50000 per la rete privata per consentire la piena funzionalità utilizzata dalla API. Se non apri queste porte, alcuni agent di monitoraggio ne risentiranno. Se si riscontrano degli errori durante la configurazione, assicurati che queste porte sano aperte prima di aprire un ticket per l'escalation.

* **openjdk** è richiesto per specifici agent di monitoraggio, come il Tomcat Monitoring Agent.
* Alcune distribuzioni Linux a 64 bit richiedono **glibc.i686** e **nss-softtokn-freebl.i686**.
* Il sistema di monitoraggio non è supportato in **FreeBSD**.

Se si verifica un errore durante la configurazione del servizio di monitoraggio dovuto ad errori di comunicazione con il robot Nimsoft, il processo di configurazione può essere messo in pausa a causa della connettività limitata. La connettività limitata è spesso causata dal firewall o da altro software di sicurezza che sta bloccando l'accesso al sistema dai server di gestione Nimsoft.  Attieniti alla seguente procedura per riavviare il provisioning del servizio di monitoraggio:

## Riavvio del provisioning di un agent di monitoraggio

1. Vai al menu **Devices** e seleziona **Monitoring**.
* Trova il sistema per cui si sta configurando il monitoraggio.
* Seleziona **"Redeploy all agents"** nel menu a discesa **Advanced** nella colonna destra.
* Scegli un template di monitoraggio nella pagina **Pop-In**.
* Fai clic su **Re-Deploy**

## Installazione in Windows
{: #install-windows}

1. Consulta http://downloads.service.softlayer.com/nimsoft/ per scaricare la versione più recente del programma di installazione Windows sul dispositivo per l'installazione (devi essere connesso alla VPN del cliente).
* Esegui il file Nimsoft Monitoring Robot come amministratore.

## Installazione in Linux
{: #install-linux}

1. Stabilisci una connessione alla rete privata tramite la VPN del cliente.
* Scarica il programma di installazione Linux a [32 bit ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} o a [64 bit ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} sul dispositivo per l'installazione. Sono disponibili anche le versioni Debian e Ubuntu nel [Nimsoft Installer ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://downloads.service.softlayer.com/nimsoft/){: new_window}.
* Esegui questi comandi per completare l'installazione, sostituendo 32 con 64, se stai eseguendo un'installazione a 64 bit.

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Passi successivi

Dopo che hai eseguito l'installazione, il sistema completa automaticamente il processo. In Windows, viene visualizzato un messaggio con una conferma di un'installazione eseguita correttamente o con le informazioni sugli eventuali errori che si sono verificati.
