---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Analyses de vulnérabilité
{{site.data.keyword.BluSoftlayer_full}} s'associe à Nessus afin de fournir des analyses de vulnérabilité pour n'importe quel périphérique sur le réseau {{site.data.keyword.BluSoftlayer_notm}}. Les analyses de vulnérabilité testent les points faibles dans un périphérique et renvoient un rapport de l'analyse, des problèmes de sécurité et des correctifs pour votre périphérique hôte. Les analyses de vulnérabilité sur vos périphériques permettent de garantir que ces derniers sont sécurisés en permanence. De plus, elles représentent la première ressource à utiliser lorsque vous pensez qu'un périphérique est vulnérable ou compromis. Les analyses de vulnérabilité peuvent être réalisées à l'aide du [portail client![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/) sur n'importe quel périphérique associé à votre compte.
{:shortdesc}

## Nessus Security Scanner 
{{site.data.keyword.BluSoftlayer_notm}} fournit un scanner de sécurité en ligne, optimisé par l'outil d'analyse Nessus open source. Ce scanner de sécurité est accessible sous l'onglet Sécurité en cliquant sur **Scanner**. Pour plus d'informations, voir [Outil d'analyse Nessus![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://www.nessus.org/nessus/).

La page **Scanner** fournit une liste de matériel disponible pour l'outil Nessus hébergé par {{site.data.keyword.BluSoftlayer_notm}}. Pour analyser un serveur, ou pour voir les résultats d'une analyse précédente, cliquez sur le lien des détails pour le serveur concerné. La page des détails de l'analyse de vulnérabilité présente rapidement le serveur (nom du serveur, adresse IP à utiliser pour l'analyse et centre de données dans lequel se trouve le serveur). Commencez à planifier l'analyse de votre serveur avec l'outil d'analyse Nessus afin de lancer une analyse de vulnérabilité le plus vite possible. 

Situé après la présentation rapide du serveur se trouve un tableau contenant les analyses de vulnérabilité Nessus en cours et précédentes. Pour chaque analyse, les informations suivantes sont spécifiées : date à laquelle l'analyse a été demandée, date à laquelle l'analyse a été demandée, état de l'analyse, aboutissement ou non de l'analyse, lien vers le rapport Nessus. 

Les états possibles pour les rapports Nessus sont les suivants :

* Analyse en attente : l'analyse a été planifiée pour le scanner Nessus. 
* Traitement de l'analyse : l'analyse est en cours de traitement. 
* Génération du rapport : l'analyse est terminée et les résultats du test sont en cours de compilation dans un rapport.
* Fin de l'analyse : l'analyse a abouti et le rapport sur les vulnérabilités a été généré. 
* Analyse annulée : l'analyse Nessus a été annulée manuellement par un technicien {{site.data.keyword.BluSoftlayer_notm}}. 

Pour toutes les analyses Nessus réussies figurant dans ce tableau, un rapport peut être affiché en cliquant sur **Afficher rapport**. Ce rapport contient deux tableaux : l'un, intitulé Détails de l'analyse de vulnérabilité, indique le nombre d'hôtes ayant été analysés, le nombre de vulnérabilités de sécurité ouvertes (trous) détectées et le nombre de vulnérabilités de sécurité potentielles (avertissements) détectées.
Le second tableau recense tous les problèmes de sécurité détectés : l'hôte sur lequel la vulnérabilité a été trouvée et une description de la vulnérabilité potentielle. 

L'outil Nessus open source est basé sur un plug-in, ce qui permet de développer de nouveaux tests à mesure que des vulnérabilités sont trouvées. {{site.data.keyword.BluSoftlayer_notm}} met régulièrement à jour l'outil Nessus interne, par conséquent, il est recommandé d'effectuer régulièrement une analyse à l'aide du scanner de sécurité pour rester informé des nouvelles menaces. 

Pour que l'analyse aboutisse, les connexions à partir des adresses 173.192.255.232 et 172.17.19.38 doivent être autorisées à accéder à votre serveur. 
