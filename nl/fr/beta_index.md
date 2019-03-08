---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# Initiation à IBM Cloud Monitoring (Bêta)
{: #gettingstartedbeta}

Cette version bêta d'application de surveillance, basée sur le service de surveillance de {{site.data.keyword.BluSoftlayer_full}}, est disponible pour les serveurs virtuels et les serveurs bare metal. Pour obtenir les mises à jour du développement de ce programme bêta, voir le [blogue IBM Cloud![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}.
{:shortdesc}

## Prérequis

Participer à ce programme bêta, vous devez répondre aux exigences suivantes :
1. Votre compte SoftLayer doit être lié à un compte IBM Cloud avec authentification par IBMid. Pour qu'un compte puisse être lié, l'utilisateur maître de votre compte SoftLayer doit se connecter à [{{site.data.keyword.slportal}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com){: new_window} et, à partir du menu **Account**, cliquer sur **Lier un compte Bluemix**.
2. Chaque utilisateur doit être lié à un ID IBM pour pouvoir consulter le programme bêta. Pour plus d'informations, voir [Liaison de comptes utilisateur IBMid](/docs/account?topic=account-unifyingaccounts#link_customer_accounts).
3. Chaque utilisateur doit avoir accès au service de surveillance IBM Cloud pour pouvoir consulter le programme bêta.
   1. A partir de la [console IBM Cloud ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://console.bluemix.net){: new_window},  sélectionnez **Gérer -> Compte -> Utilisateurs**.
   2. Invitez l'utilisateur sur le compte ou sélectionnez-le dans la liste.
   3. Sélectionnez **Affecter l'accès aux ressources** pour l'utilisateur.
   4. Dans **Service**, sélectionnez **IBM Cloud Monitoring Service**.
   5. Sélectionnez le **rôle** à accorder à l'utilisateur pour toutes les régions.

Si ces conditions ne sont pas réunies, vous ne pouvez pas accéder au programme de surveillance bêta.


## Comment rejoindre le programme bêta

Procédez comme indiqué ci-après pour commencer à utiliser le programme bêta de surveillance. Lorsque vous rejoignez le programme bêta, le service de surveillance est activé pour tous les serveurs virtuels et bare metal éligibles dans votre compte. Le fait de cliquer sur Rejoignez le programme bêta n'affecte pas la surveillance ou les données Nimsoft existantes.
1. (Bare metal uniquement) [Installez l'agent de surveillance sur votre serveur bare metal](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-).
<table>
   <CAPTION>Tableau 1. Choix d'un emplacement de connexion</CAPTION>
   <THEAD>
   <TR>
   <th>Pour rejoindre le programme bêta via le...</th>
   <th>Procédure</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Catalogue IBM Cloud</td>
   <td>
   <ol>
   <li>Ouvrez une fenêtre de navigateur et entrez <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>.</li>
   <li>Cliquez sur le lien <b>Se connecter</b>. </li>
   <li>Entrez votre adresse électronique ou votre ID IBM puis cliquez sur <b>Continuer</b>.</li>
   <li>Entrez votre mot de passe, puis cliquez sur <b>Se connecter</b>.</li>
   <li>Sélectionnez **Infrastructure->Liste des unités->*Nom d'unité*** pour accéder aux détails du périphérique.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Portail client</td>
   <td>
   <ol>
   <li>Ouvrez une nouvelle fenêtre de navigateur et entrez <a href="https://control.softlayer.com">https://control.softlayer.com</a>.</li>
   <li>Entrez votre nom d'utilisateur et votre mot de passe, puis cliquez sur <b>Se connecter</b>. Ou, cliquez sur <b>Connexion par ID IBM</b>. Entrez ensuite votre adresse électronique ou votre ID IBM puis cliquez sur <b>Continuer</b>. Entrez votre mot de passe, puis cliquez sur <b>Se connecter</b>. La page principale du portail {{site.data.keyword.slportal}} s'affiche.</li>
     <li>Dans **Unités**, cliquez sur **Nom d'unité** pour accéder aux détails du périphérique.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. Sélectionnez **Unités -> Surveillance**. Cliquez sur **Rejoignez le programme bêta** pour afficher les onglets bêta des règles système et des notifications.

## Etapes suivantes
1. Passez en revue les détails des [métriques](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-) collectées.
2. [Créez ou gérez](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-) une notification de moniteur.
3. [Créez ou gérez](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-) une règle système.
4. [Affichez des alertes](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-).
5. Passez en revue les données du graphique de surveillance bêta actuellement disponibles pour un périphérique sélectionné.

|              Métriques                                      |  Description                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|Utilisation de l'UC                                            |   Permet d'afficher le % d'utilisation de l'UC pour chaque coeur et une moyenne entre les coeurs. Cliquez sur chaque métrique dans la clé pour activer ou désactiver les données sur le graphique.
|Réseau public                                             |   Permet d'afficher les données entrantes et sortantes pour votre réseau public. Cliquez sur chaque métrique dans la clé pour activer ou désactiver les données sur le graphique.       |
|Réseau privé                                            |   Permet d'afficher les données entrantes et sortantes pour votre réseau privé. Cliquez sur chaque métrique dans la clé pour activer ou désactiver les données sur le graphique.           |
|Utilisation de la mémoire    | Permet d'afficher le % d'utilisation de la mémoire pour votre serveur     |
|Utilisation du disque    | Permet d'afficher la quantité moyenne (en octets) de données lues ou écrites depuis ou sur un disque ou le temps d'attente du disque. Cliquez sur chaque métrique dans la clé pour activer ou désactiver les données sur le graphique.    |
|Température                                                 |Permet d'afficher la température de votre périphérique bare metal en degrés Celsius. Ces données ne sont pas disponibles pour tous les périphériques.
{: caption="Tableau 1. Métriques bêta" caption-side="top"}   

## Limitations
Si un périphérique est supprimé, les règles de surveillance qui lui sont associées ne sont pas supprimées. Sachez que vous devez supprimer manuellement le périphérique pour que ces règles soient également supprimées.

Les données de métrique ne sont disponibles que pendant 15 jours.

Il ne peut exister que 10 règles de surveillance à la fois. Toutefois, une règle peut être appliquée à plusieurs périphériques.

## Identification et résolution des problèmes
L'affichage de certaines métriques, telles que l'utilisation de la mémoire, requiert la présence d'outils Xen sur votre serveur. Pour plus d'informations sur l'installation d'outils Xen, voir [Préparation et importation d'images](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images).

## Commentaires
Pour envoyer vos commentaires sur ce programme bêta, sélectionnez **Unités - >Surveillance** ou la page des détails de l'unité, puis cliquez sur **Déposer un commentaire** pour répondre à une enquête rapide. Pour quitter le programme bêta et revenir à la vue standard, cliquez sur le lien **Quitter le programme bêta** au bas de la page **Unités -> Surveillance**.
