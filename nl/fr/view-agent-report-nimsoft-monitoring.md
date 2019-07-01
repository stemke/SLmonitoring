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

# Affichage d'un rapport d'agent pour la surveillance Nimsoft
{: #viewing-an-agent-report-for-nimsoft-monitoring}

Les détails de la surveillance Nimsoft sont disponibles dans des rapports d'agent. Ces derniers contiennent des détails relatifs à la façon dont l'agent a été configuré. 
{:shortdesc}

## Avant de commencer
Tout d'abord, naviguez jusqu'au menu de l'appareil et assurez-vous d'avoir les autorisations de compte appropriées pour effectuer les tâches.

* Accédez au menu de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Vérifiez que vous disposez des autorisations de compte nécessaires et que vous avez accès à l'appareil. Seul le propriétaire du compte, ou un utilisateur avec l'autorisation **Gérer les utilisateurs** de l'infrastructure classique, peut régler les autorisations.

Pour plus d'informations sur les autorisations, voir [Droits d'infrastructure classique](/docs/iam?topic=iam-infrapermission#infrapermission) et [Gestion de l'accès aux terminaux](/docs/vsi?topic=virtual-servers-managing-device-access).

## Affichage d'un rapport d'agent pour la surveillance Nimsoft
{: #viewing-agent-report-nimsoft-monitoring-steps}

Pour afficher un rapport d'état pour la surveillance Nimsoft, procédez comme suit :

1. Sur la page **Surveillance**, sélectionnez **Afficher les rapports d'agent** dans le menu **Actions**.
2. Sélectionnez l'agent à afficher dans la liste **Agents**.

  Les agents disponibles varient d'un appareil à un autre et dépendent du module de surveillance appliqué à l'appareil.
  {:note}
  
3. Accédez à toutes les autres sections et exécutez notamment une ou plusieurs des actions suivantes :

  Chaque agent est différent et ne comporte pas toutes les sections ou métriques. Les options disponibles sur cet écran dépendent des options de configuration disponibles pour chaque agent.
  {:note}
  
  * Sélectionnez le rapport de section dans la liste **Sections**.
  * Sélectionnez la période pour le rapport dans la liste **Afficher par** .
  * Cochez la case correspondant à chaque métrique que vous souhaitez inclure dans le rapport, dans la section **Sélectionnez les métriques pour lesquelles générer un rapport**.
    
    Seules des métriques similaires apparaissent sur le même diagramme. Si des métriques conflictuelles sont choisies, une erreur se produit lorsque vous demandez le diagramme.
    {:note}
4. Cliquez sur **Dessiner un diagramme** pour dessiner le diagramme.

## Etapes suivantes

Une fois le diagramme dessiné pour le rapport d'agent, il peut être redessiné à tout moment pour afficher différentes métriques en répétant ces étapes. Le nombre de rapports d'agent pouvant être créés dans un laps de temps défini est illimité.
