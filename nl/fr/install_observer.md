---

copyright:
  years: 2018
lastupdated: "2018-04-20"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installation d'IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Bêta)

Afin de permettre à la surveillance avancée de fonctionner sur un périphérique {{site.data.keyword.baremetal_short}} existant, procédez comme indiqué ci-après pour installer {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent sur votre périphérique bare metal.

## Prérequis
Vous devez être connecté à votre périphérique bare metal pour télécharger et exécuter les programmes d'installation.

## Installation sous Windows

1. Téléchargez le programme d'installation d'IBM Cloud Monitoring Agent pour Windows. [Télécharger![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi){: new_window}
2. Exécutez le programme d'installation sur la machine cible.

## Installation sous Linux

1. Téléchargez le programme d'installation d'IBM Cloud Monitoring Agent pour Linux. [Télécharger![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz){: new_window}
2. Extrayez-le sur la machine cible.
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. Exécutez le script linux_install.sh.


## Installation sous FreeBSD
1. Téléchargez le programme d'installation d'IBM Cloud Monitoring Agent pour FreeBSD. [Télécharger![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz){: new_window}
2. Extrayez-le sur la machine cible.
  `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. Exécutez le script freebsd_install.sh.

## Etapes suivantes

Après que vous avez exécuté l'installation, le système achève le processus automatiquement. Sous Windows, un message s'affiche pour confirmer que l'installation a abouti ou pour signaler que des erreurs se sont produites.

Si vous utilisez un pare-feu, vous devrez peut-être autoriser IBM Cloud Monitoring Agent à transmettre des données via ce pare-feu. L'agent utilise le port 8090 pour la communication HTTPS sortante. Pour plus d'informations sur les adresses IP pour lesquelles vous devrez peut-être activer des autorisations, voir [Load balancer IP ranges](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-load-balancer-ips#load-balancer-ips).
