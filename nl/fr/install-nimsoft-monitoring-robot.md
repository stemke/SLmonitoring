---

copyright:
  years: 2014, 2019
lastupdated: "2019-02-11"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installation et gestion de Nimsoft Monitoring Robot

Afin de permettre à la surveillance avancée de fonctionner sur un périphérique {{site.data.keyword.baremetal_short}} ou {{site.data.keyword.BluVirtServers_short}} existant, installez Nimsoft Monitoring Robot. Nimsoft Monitoring Robot permet au système de gestion de la surveillance de communiquer avec le serveur bare metal ou le serveur virtuel sur le réseau privé. Une fois Nimsoft Monitoring Robot installé, il faut environ 5 à 10 minutes pour qu'il devienne disponible sur le portail {{site.data.keyword.slportal_full}}. Procédez comme indiqué ci-après pour installer Nimsoft Monitoring Robot sous Windows ou Linux.

## Prérequis

Avant de procéder à l'installation, les ports suivants doivent être ouverts sur le réseau privé :

* tcp/48000
* tcp/48001
* tcp/48002

En outre, ouvrez les portes tcp/48003 à tcp/50000 pour le réseau privé afin de permettre la fonctionnalité complète qui est utilisée par l'API. Si vous n'ouvrez pas ces ports, certains agents de surveillance sont affectés. Si des erreurs sont détectées lors de la configuration, vérifiez que ces ports sont ouverts avant d'ouvrir et de soumettre un ticket.

* **openjdk** est requis pour certains agents de surveillance, tels que Tomcat Monitoring Agent.
* Certaines distributions Linux 64 bits requièrent **glibc.i686** et **nss-softtokn-freebl.i686**.
* Le système de surveillance n'est pas pris en charge dans **FreeBSD**.

Si une erreur se produit lors de la configuration du service de surveillance en raison d'erreurs de communication avec le robot Nimsoft, le processus de configuration peut être suspendu en raison de la connectivité limitée. Cela est souvent dû à un pare-feu ou à d'autres logiciels de sécurité qui bloquent l'accès au système à partir des serveurs de gestion Nimsoft.  Procédez comme suit pour redémarrer la mise à disposition du service de surveillance :

## Redémarrage de la mise à disposition d'un agent de surveillance

1. Accédez au menu **Unités** et sélectionnez **Surveillance**.
* Recherchez le système pour lequel la surveillance est en cours de configuration.
* Sélectionnez **"Redéployer tous les agents"** dans la liste déroulante **Avancé** dans la colonne de droite.
* Choisissez un modèle de surveillance sur la page **contextuelle**.
* Cliquez sur **Redéployer**

## Installation sous Windows

1. Accédez à http://downloads.service.softlayer.com/nimsoft/ pour télécharger la dernière version de Windows Installer sur le périphérique pour installation (vous devez être connecté au réseau privé virtuel du client).
* Exécutez le fichier Nimsoft Monitoring Robot en tant qu'administrateur.

## Installation sous Linux

1. Connectez-vous au réseau privé via le réseau privé virtuel du client. 
* Téléchargez le programme d'installation Linux [32 bits ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} ou [64 bits ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} sur le périphérique pour installation. Les versions Debian et Ubuntu sont également disponibles sur [Nimsoft Installer ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://downloads.service.softlayer.com/nimsoft/){: new_window}.
* Exécutez les commandes suivantes pour effectuer l'installation, en remplaçant 32 par 64, si vous exécutez une installation 64 bits :

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Etapes suivantes

Après que vous avez exécuté l'installation, le système achève le processus automatiquement. Sous Windows, un message s'affiche pour confirmer que l'installation a abouti ou pour signaler que des erreurs se sont produites.
