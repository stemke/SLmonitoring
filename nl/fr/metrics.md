---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Métriques collectées (Bêta)
Cette rubrique présente les métriques collectées pour cette version bêta d'application de surveillance sur les serveurs virtuels et les serveurs bare metal.
{:shortdesc}

Cette rubrique décrit toutes les métriques disponibles via des requêtes Grafana. Pour plus d'informations, voir [Création d'une requête de surveillance avancée (Bêta)](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-an-advanced-monitoring-query-beta-#creating-an-advanced-monitoring-query-beta-). Des diagrammes sont disponibles dans l'interface utilisateur uniquement pour les métriques suivantes :
* Utilisation de l'UC
* Utilisation de la mémoire
* Lecture et écriture sur disque (octets/secondes et E-S par seconde)
* Temps d'attente d'écriture et de lecture sur disque
* Débit de réseau public (entrant/sortant)
* Débit de réseau privé (entrant/sortant)
* Paquets de réseau public (entrants/sortants) (serveurs bare metal uniquement)
* Paquets de réseau privé (entrants/sortants) (serveurs bare metal uniquement)
* Erreurs de réseau public (entrantes/sortantes) (serveurs bare metal uniquement)
* Erreurs de réseau privé (entrantes/sortantes) (serveurs bare metal uniquement)
* Température (serveurs bare metal uniquement)


## Métriques d'unité centrale
  Les métriques d'unité centrale mesurent le pourcentage moyen du temps nécessaire à une unité centrale pour exécuter des instructions pendant une période donnée. Le pourcentage moyen d'inactivité porte sur l'inactivité relative à l'ajout d'utilisateur, à nice, au système, au temps d'attente des E-S, aux interruptions de matériel et aux interruptions logicielles

## Métriques de la mémoire
* Octets utilisés/Moyenne d'utilisation : quantité de mémoire utilisée à un moment donné, disponible en octets et en pourcentage du total.
* Octets de permutation utilisés/Moyenne d'utilisation : pourcentage de mémoire de permutation utilisé durant une période donnée. Cette métrique est une indication de la fréquence à laquelle vous devez extraire des données qui ne sont pas en mémoire. Cette métrique est disponible uniquement sur les périphériques bare metal.

## Métriques de disque

* Total disque : nombre total d'octets disponibles sur le disque. Cette métrique doit être constante.
* Disque utilisé (octets) : nombre d'octets utilisés par le disque au moment indiqué. 
* Disque utilisé (pourcentage) : pourcentage du nombre total d'octets utilisé par rapport au nombre total d'octets disponibles sur le disque. 
* Lecture/écriture sur disque (octets/seconde) : quantité moyenne de données lues/écrites depuis/sur un disque, exprimée en octets et pour une période donnée.
* Lecture/écriture sur disque (opérations/seconde) : opérations de lecture/écriture par seconde.
* Lecture/écriture sur disque (temps d'attente en milliseconde par opération) : temps d'attente en milliseconde par opération de lecture/écriture.

## Métriques de réseau

 * Réseau public/privé (entrant) : nombre d'octets reçus par le réseau public/privé.
* Réseau public/privé (sortant) : nombre d'octets envoyés par le réseau public/privé.
* Paquets entrants dans réseau public/privé : nombre de paquets reçus par l'interface réseau du réseau public/privé. Cette métrique est disponible uniquement sur les périphériques bare metal.
* Paquets sortants de réseau public/privé : nombre de paquets envoyés par l'interface réseau du réseau public/privé. Cette métrique est disponible uniquement sur les périphériques bare metal.

## Métriques de température
* Température moyenne du système, mesurée en degrés celsius. Cette métrique est disponible uniquement sur certains périphériques bare metal.
