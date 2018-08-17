---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# Foire aux questions relatives à la surveillance

<a name="48"></a>
## Je vois de nombreux tickets d'alerte de surveillance. Cela signifie-t-il que mon serveur est en panne ?

Chaque périphérique est livré avec un service de notification et de ping de surveillance gratuit. Ce service crée automatiquement un ticket d'alerte si des paramètres définis échouent. Des faux positifs peuvent être générés par le service de surveillance et se voir attribuer une limitation de taux par un pare-feu logiciel sur le serveur, pour la disponibilité d'application et de service et les interruptions de service dans l'infrastructure de surveillance. Vérifiez les paramètres par défaut en vue de réduire le nombre de fausses alertes de surveillance possibles. 

<a name="354"></a>
## Puis-je faire en sorte que le système de surveillance exécute un redémarrage automatique et envoie une alerte à un technicien de support si le serveur ne répond plus ?

Oui, le service **Redémarrage automatisé en cas d'échec de la surveillance** vous permet de configurer le système de surveillance pour redémarrer automatiquement le serveur et envoyer un ticket au technicien de support si une alerte de surveillance est émise.  

<a name="1699"></a>
## Quelle est la différence entre la surveillance avec une "demande ping lente" et la surveillance avec une "demande ping de service" ?

La différence entre une demande ping de service et une demande ping lente réside dans délai pendant lequel une réponse provenant du périphérique est attendue. Par défaut, une demande ping de service est utilisé, mais vous pouvez choisir d'utiliser une demande ping lente à la place. 

* Une demande ping de **service** est émise toutes les 5 minutes et s'attend à recevoir une réponse d'écho dans un délai d'1 seconde. Si plusieurs demandes ping sont manquées, une alerte est émise. 
* Une demande ping **lente** attend une réponse pendant 5 secondes, accordant ainsi aux serveurs qui sont optimisés pour des tâches hors réseau davantage de temps pour traiter la demande. 


<a name="1000"></a>
## Lorsqu'un ticket de surveillance est ouvert et me prévient qu'un problème s'est produit, ce ticket est-il visible par les techniciens et ces derniers peuvent-ils y répondre ?

Avec le service ping de base, les techniciens de support ne sont pas avertis des incidents. Ces tickets sont ouverts lorsque le système de surveillance émet une alerte, mais ils n'avertissent que les utilisateurs indiqués sur l'écran de surveillance. Les techniciens ne sont avertis que si vous ouvrez un nouveau ticket pour indiquer que le serveur ne répond pas. 

