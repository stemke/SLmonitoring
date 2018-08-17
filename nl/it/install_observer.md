---
copyright:
  years: 2018
lastupdated: "2018-04-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installazione di IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)

Per consentire il funzionamento del monitoraggio avanzato sul {{site.data.keyword.baremetal_short}} esistente, attieniti alla seguente procedura per installare {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent sul tuo dispositivo bare metal.

## Prerequisiti
Devi essere connesso al tuo dispositivo bare metal per scaricare ed eseguire i programmi di installazione.

## Installazione in Windows

1. Scarica il programma di installazione di Windows IBM Cloud Monitoring Agent. [Download](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi)
2. Esegui il programma di installazione sulla macchina di destinazione. 

## Installazione in Linux

1. Scarica il programma di installazione di Linux IBM Cloud Monitoring Agent. [Download](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz)
2. Decomprimilo sulla macchina di destinazione.
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. Esegui lo script linux_install.sh.

        
## Installazione in FreeBSD
1. Scarica il programma di installazione di FreeBSD IBM Cloud Monitoring Agent. [Download](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz)
2. Decomprimilo sulla macchina di destinazione.
       `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. Esegui lo script freebsd_install.sh. 

## Passi successivi

Dopo che hai eseguito l'installazione, il sistema completa automaticamente il processo. In Windows, viene visualizzato un messaggio con una conferma di un'installazione eseguita correttamente o con le informazioni sugli eventuali errori che si sono verificati.

Se stai utilizzando un firewall, potresti dover consentire a IBM Cloud Monitoring Agent di passare i dati attraverso di esso. L'agent utilizza la porta 8090 per le comunicazioni HTTPS in uscita. Per ulteriori informazioni sugli indirizzi IP che potresti dover consentire, consulta [Load balancer IP ranges](https://console.bluemix.net/docs/infrastructure/hardware-firewall-dedicated/ips.html#load-balancer-ips).
