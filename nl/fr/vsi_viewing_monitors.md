---

copyright:
  years: 2017, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:note: .note}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Affichage et gestion des moniteurs
{: #viewing-and-managing-monitors}

La surveillance d'un périphérique vous permet d'initier des demandes ping de service et des demandes ping lentes de sorte que ce périphérique soit en ligne et réactif.
{:shortdesc}

Si aucun écho n'est reçu pendant la période allouée (1 seconde pour les demandes ping de service, 5 secondes pour les demandes ping lentes), une alerte est envoyée à
l'adresse électronique du compte. Lorsque la zone **Etat** indique **Actif**, cela signifie qu'un écho a été reçu, tandis que lorsqu'elle indique **Arrêté**, cela signifie que l'écho n'a pas été reçu. Si vous disposez d'un moniteur de base configuré, procédez comme suit pour afficher et gérer la surveillance d'un périphérique :

## Avant de commencer
Tout d'abord, naviguez jusqu'au menu de l'appareil et assurez-vous d'avoir les autorisations de compte appropriées pour effectuer les tâches.

* Accédez au menu de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Vérifiez que vous disposez des autorisations de compte nécessaires et que vous avez accès à l'appareil. Seul le propriétaire du compte, ou un utilisateur avec l'autorisation **Gérer les utilisateurs** de l'infrastructure classique, peut régler les autorisations.

Pour plus d'informations sur les autorisations, voir [Droits d'infrastructure classique](/docs/iam?topic=iam-infrapermission#infrapermission) et [Gestion de l'accès aux terminaux](/docs/vsi?topic=virtual-servers-managing-device-access).

## Affichage des moniteurs
{: #viewing-monitors}

1. Dans le menu **Unités**, sélectionnez **Liste d'unités**.
2. Cliquez sur le nom de l'élément auquel vous souhaitez accéder.
3. Cliquez sur l'onglet **Surveillance**. Toutes les demandes ping ne sont pas visibles sur la page d'arrivée.

L'onglet **Surveillance** est visible uniquement si au moins un moniteur est configuré.
{:note}

## Ajout d'un moniteur
{: #adding-a-monitor}

1. Dans le menu **Unités**, sélectionnez **Liste d'unités**.
2. Cliquez sur le nom de l'élément auquel vous souhaitez accéder.
3. Cliquez sur l'onglet **Surveillance** puis sélectionnez **Gérer les moniteurs**.
4. Sélectionnez **Ajouter moniteur**.
5. Sélectionnez l'adresse IP à surveiller dans la zone **Adresse IP** ainsi que le type de moniteur dans la zone **Type de moniteur**.  
6. Configurez les options de notification. Dans la zone **Avertir ?**, sélectionnez **Notifier les utilisateurs** pour avertir les utilisateurs de problèmes, ou **Ne rien faire** pour ignorer la notification utilisateur.
7. Sélectionnez le délai pour la notification utilisateur dans la zone **Notifier attente**. 
8. Cliquez sur **Ajouter moniteur** afin d'ajouter le moniteur au périphérique. Le nouveau moniteur s'affiche dans la section **Editer les superviseurs existants**.

## Edition d'un moniteur existant
{: #editing-an-exisiting-monitor}

1. Dans le menu **Unités**, sélectionnez **Liste d'unités**.
2. Cliquez sur le nom de l'élément auquel vous souhaitez accéder.
3. Cliquez sur l'onglet **Surveillance** puis sélectionnez **Gérer les moniteurs**.
4. Dans la section **Editer les superviseurs existants**, cliquez sur un des détails de moniteur pour ouvrir ce dernier afin de pouvoir l'éditer.
5. Mettez à jour une des zones suivantes : **Type de moniteur, Notifier** ou **Notifier attente**.
6. Cliquez sur **Mettre à jour** pour mettre à jour les détails.

## Retrait d'un moniteur
{: #removing-a-monitor}

1. Dans le menu **Unités**, sélectionnez **Liste d'unités**.
2. Cliquez sur le nom de l'élément auquel vous souhaitez accéder.
3. Cliquez sur l'onglet **Surveillance** puis sélectionnez **Gérer les moniteurs**.
4. Dans la section **Editer les superviseurs existants**, cliquez sur l'icône **Retirer** dans les détails du moniteur.
5. Sélectionnez **Oui** pour retirer le moniteur.

## Etapes suivantes

- Si un nouveau moniteur est ajouté, il apparaît sur l'onglet **Surveillance**. Le moniteur envoie une demande ping au périphérique toutes les 5 minutes et s'attend à recevoir une réponse qui varie en fonction de type de demande ping sélectionné. Si la réponse attendue n'est pas reçue, un courrier électronique est envoyé à l'adresse électronique de notification pour le compte dans le délai indiqué, si l'option de notification est sélectionnée.
- Si un moniteur est édité, il continue de fonctionner comme indiqué dans les détails le concernant. Si le type est modifié, le délai d'attente pour la réception de la demande ping attendue est différent. Si les options de notification sont modifiées, la façon dont les utilisateurs sont avertis qu'une tentative a échoué change en fonction des nouvelles sélections. Le moniteur reste accessible depuis l'onglet **Surveillance**.
- Si un moniteur est retiré, il ne fonctionne plus pour le périphérique. La surveillance qui est associée au moniteur retiré s'arrête complètement et ce dernier n'apparaît plus dans l'onglet **Surveillance**.

