---

copyright:
  years: 2014, 2018
lastupdated: "2018-11-15"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Surveillance
{: #monitoring}

{{site.data.keyword.BluSoftlayer_full}} inclut des services de surveillance Standard et des services de surveillance Nimsoft. Ainsi, vous avez connaissance à tout moment des problèmes pouvant survenir sur vos périphériques. Les services de surveillance Standard incluent des fonctions telles que Ping et Statistiques IPMI. La surveillance Nimsoft inclut trois niveaux de surveillance : de base, avancé et premium. Chaque service au sein des offres de surveillance Standard et Nimsoft fournit différents avantages et est proposé à différents tarifs en fonction de vos besoins métier. Pour plus d'informations, voir [{{site.data.keyword.cloud}} infrastructure monitoring & reporting ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}.

La surveillance d'un périphérique permet aux utilisateurs d'initier des demandes ping de service et des demandes ping lentes de sorte que ce périphérique soit en ligne et réactif.

Si aucun écho n'est reçu pendant la période allouée (1 seconde pour les demandes ping de service, 5 secondes pour les demandes ping lentes), une alerte est envoyée à
l'adresse électronique du compte. Lorsque la zone **Statut** indique **Actif**, cela signifie qu'un écho a été reçu, tandis que lorsqu'elle indique **Arrêté**, cela signifie que l'écho n'a pas été reçu.

Pour afficher des moniteurs configurés, procédez comme suit :

1. Dans la liste des unités, cliquez sur le **Nom de l'unité** pour accéder à cet élément.

2. Cliquez sur l'onglet **Surveillance**. Toutes les demandes ping ne sont pas visibles sur la page d'arrivée. (L'onglet **Surveillance** est visible uniquement si au moins un moniteur est configuré.)
