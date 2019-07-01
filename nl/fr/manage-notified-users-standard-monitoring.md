---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestion des utilisateurs avertis pour la surveillance standard
{: #managing-notified-users-for-standard-monitoring}

Les utilisateurs avertis pour le service de surveillance standard reçoivent des notifications automatisées chaque fois qu'un périphérique ne répond pas à une demande ping dans le délai imparti. Vous pouvez ajouter ou retirer des utilisateurs avertis à tout moment, et les utilisateurs avertis doivent figurer sur le compte qui est associé au périphérique pour recevoir une notification. Procédez comme indiqué ci-après afin de gérer les utilisateurs avertis pour le service de surveillance standard.
{:shortdesc}

## Avant de commencer
Tout d'abord, naviguez jusqu'au menu de l'appareil et assurez-vous d'avoir les autorisations de compte appropriées pour effectuer les tâches.

* Accédez au menu de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Vérifiez que vous disposez des autorisations de compte nécessaires et que vous avez accès à l'appareil. Seul le propriétaire du compte, ou un utilisateur avec l'autorisation **Gérer les utilisateurs** de l'infrastructure classique, peut régler les autorisations.

Pour plus d'informations sur les autorisations, voir [Droits d'infrastructure classique](/docs/iam?topic=iam-infrapermission#infrapermission) et [Gestion de l'accès aux terminaux](/docs/vsi?topic=virtual-servers-managing-device-access).

## Ajout d'utilisateurs notifiés
{: #adding-notified-users}

Procédez comme suit pour ajouter des utilisateurs notifiés pour le service de surveillance standard.
1. Dans le menu **Unité**, sélectionnez **Liste des unités**.
2. Cliquez sur le nom de l'élément auquel vous souhaitez accéder.
3. Cliquez sur l'onglet **Surveillance** puis sélectionnez **Gérer les moniteurs**.
4. Sélectionnez **Gérer les utilisateurs avertis**.
5. Dans la liste déroulante **Utilisateurs à avertir**, sélectionnez l'utilisateur auquel envoyer une notification.
6. Sélectionnez **Ajouter un utilisateur**.

## Retrait d'utilisateurs notifiés
{: #removing-notified-users}

Procédez comme suit pour retirer des utilisateurs notifiés pour le service de surveillance standard.
1. Dans le menu **Unité**, sélectionnez **Liste des unités**.
2. Cliquez sur le nom de l'élément auquel vous souhaitez accéder.
3. Cliquez sur l'onglet **Surveillance** puis sélectionnez **Gérer les moniteurs**.
4. Sélectionnez **Gérer les utilisateurs avertis**.
5. Cliquez sur l'icône **Retirer** pour retirer l'utilisateur notifié existant puis sélectionnez **Oui** pour retirer l'utilisateur. 

## Etapes suivantes

Si vous ajoutez un utilisateur notifié, ce dernier est averti en cas de réponse manquée à une demande ping. Si vous avez retiré un utilisateur notifié, ce dernier ne reçoit plus de notification concernant une réponse manquée à une demande ping qui est associée à l'appareil.
