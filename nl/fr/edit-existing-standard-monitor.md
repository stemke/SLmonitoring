---
copyright:
  years: 1994, 2017
lastupdated: "2018-05-18"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Edition d'un moniteur existant
Une fois qu'un moniteur est ajouté à un périphérique, vous pouvez le modifier ou le retirer à tout moment. Il est possible de modifier le type et les options de notification d'un moniteur, mais le fait de retirer un moniteur annule complètement celui-ci. Procédez comme indiqué ci-après pour éditer un moniteur existant. 

1\. Sur la page **Moniteurs** sous l'en-tête **Editer les superviseurs existants**, cliquez sur n'importe quels détails de moniteur pour ouvrir le moniteur afin de pouvoir l'éditer. 

2\. Modifiez les **détails de moniteur** si besoin. Reportez-vous au tableau suivant pour en savoir plus sur chacune des zones modifiables :

<caption>Tableau 1. Description des zones modifiables</caption> 
|Zone|Détails|Action|
|---|---|---|
|Type de moniteur|Délai pendant lequel une réponse provenant du périphérique est attendue. Le système utilise par défaut une demande ping de service. Une demande ping lente attend une réponse pendant 5 secondes, accordant ainsi aux serveurs qui sont optimisés pour des tâches hors réseau davantage de temps pour traiter la demande. Une demande ping de service est émise toutes les 5 minutes et s'attend à recevoir une réponse d'écho dans un délai d'1 seconde. Si plusieurs demandes ping sont manquées, une alerte est émise. |Sélectionnez **Ping lent** ou **Ping de service**.|
|Notifier|Les utilisateurs avertis reçoivent des notifications automatisées chaque fois qu'un périphérique ne répond pas à une demande ping dans le délai imparti. Un utilisateur doit figurer sur le compte qui est associé au périphérique pour recevoir une notification. |Pour ajouter un utilisateur, sélectionnez **Utilisateur averti**, puis cliquez sur **Ajouter un utilisateur**. Pour retirer un utilisateur, cliquez sur l'icône **Retirer** en regard de l'utilisateur averti existant, puis cliquez sur **Oui** pour confirmer votre action. |
|Notifier attente|Délai d'attente observé par le système avant d'envoyer une notification lorsque le périphérique ne répond pas à une demande ping. Plusieurs délais d'attente sont disponibles. **Remarque :** les détails de notification ne sont pas requis lorsqu'aucun utilisateur n'est sélectionné pour notification. |Sélectionnez le délai d'attente dont vous avez besoin.|

3\. Cliquez sur **Mettre à jour** pour appliquer les modifications au moniteur. Cliquez sur **Annuler** pour annuler l'action.

## Etapes suivantes

Si un moniteur est édité, il continue de fonctionner comme indiqué dans les détails le concernant. Si le type est modifié, le délai d'attente pour la réception de la demande ping attendue est différent. Si les options de notification changent, le mode de notification change en fonction des nouvelles sélections. Le moniteur reste accessible depuis l'onglet Surveillance. 
