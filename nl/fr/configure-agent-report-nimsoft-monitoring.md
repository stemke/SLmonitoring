---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configuration d'un rapport d'agent de surveillance Nimsoft
{: #configuring-a-nimsoft-monitoring-agent-report}

## Avant de commencer

Tout d'abord, naviguez jusqu'au menu de l'appareil et assurez-vous d'avoir les autorisations de compte appropriées pour effectuer les tâches.

* Accédez au menu de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Vérifiez que vous disposez des autorisations de compte nécessaires et que vous avez accès à l'appareil. Seul le propriétaire du compte, ou un utilisateur avec l'autorisation **Gérer les utilisateurs** de l'infrastructure classique, peut régler les autorisations.

Pour plus d'informations sur les autorisations, voir [Droits d'infrastructure classique](/docs/iam?topic=iam-infrapermission#infrapermission) et [Gestion de l'accès aux terminaux](/docs/vsi?topic=virtual-servers-managing-device-access).

## Configuration d'un rapport d'agent de surveillance Nimsoft
{: #configuring-nimsoft-monitoring-agent-report-steps}

Procédez comme suit pour configurer un rapport d'agent Nimsoft Monitoring.

1. Dans le menu **Unités**, sélectionnez **Surveillance**.
2. Sur la page **Surveillance**, sélectionnez **Configurer les rapports d'agent** dans le menu déroulant **Actions** de la colonne **Avancé**.
3. Sélectionnez l'agent à configurer dans la liste déroulante **Agents**.
  
  Les agents disponibles varient d'un appareil à un autre et dépendent du module de surveillance appliqué à l'appareil.
  {:note}

4. Sélectionnez la section à configurer dans la liste déroulante **Sections**. Si vous sélectionnez une section qui contient des profils, une autre liste déroulante s'affiche. Dans cette liste, sélectionnez un **profil existant** dans la liste déroulante **Profils**. Pour ajouter une nouvelle configuration, sélectionnez **Ajouter une config agent...** dans la liste déroulante **Profils**.

5. Renseignez chaque zone de la section **Métriques générales et informations**, si besoin.
  
  Les zones obligatoires sont signalées par un astérisque rouge (*). Cette section ne figure pas dans tous les agents, sections ou profils.
  {:note}

6. Cochez la case **Métriques** pour chaque métrique à inclure dans le rapport à partir de la section **Sélectionnez les métriques pour lesquelles générer un rapport**, le cas échéant.

7. Cochez la case **Alarme** pour chaque alarme à activer pour l'agent dans **Alarmes de métrique**.

  Les alarmes de cette section ne sont pas toutes liées à une métrique spécifique. Les alarmes sont envoyées à chaque adresse électronique associée à la section **Abonnés à l'alarme** pour l'agent.
  {:note}

7. Cliquez sur **Sauvegarder** pour sauvegarder la configuration. Cliquez sur **Annuler** pour annuler l'action.
  
  Le bouton **Sauvegarder** est désactivé jusqu'à ce que vous apportiez une modification à la configuration en cours.
  {:note}

## Etapes suivantes

Une fois la configuration sauvegardée, une message de confirmation s'affiche. Si la configuration a échoué, un message d'erreur s'affiche avec une description de l'erreur qui s'est produite et la procédure à suivre pour la résoudre. Vous pouvez reconfigurer des agents à tout moment en répétant ces étapes.
