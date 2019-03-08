---

copyright:
  years: 2017
lastupdated: "2017-09-28"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Affichage et gestion des moniteurs

La surveillance d'un périphérique permet aux utilisateurs d'initier des demandes ping de service et des demandes ping lentes de sorte que ce périphérique soit en ligne et réactif.
{:shortdesc}

Si aucun écho n'est reçu pendant la période allouée (1 seconde pour les demandes ping de service, 5 secondes pour les demandes ping lentes), une alerte est envoyée à
l'adresse électronique du compte. Lorsque la zone **Etat** indique **Actif**, cela signifie qu'un écho a été reçu, tandis que lorsqu'elle indique **Arrêté**, cela signifie que l'écho n'a pas été reçu. Si vous disposez d'un moniteur de base configuré, procédez comme suit pour afficher et gérer la surveillance d'un périphérique :

   <table>
   <CAPTION>Tableau 1. Affichage et gestion de la surveillance de périphérique</CAPTION>
   <THEAD>
   <TR>
   <th>Action</th>
   <th>Procédure</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Affichage des moniteurs</td>
   <td>
   <ol>
   <li>Dans la liste des unités, cliquez sur le <b>Nom de l'unité</b> pour accéder à cet élément.</li>
   <li>Cliquez sur l'onglet <b>Surveillance</b>. Toutes les demandes ping ne sont pas visibles sur la page d'arrivée. (L'onglet <b>Surveillance</b> est visible uniquement si au moins un moniteur est configuré.)</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Ajout d'un moniteur</td>
   <td>
   <ol>
   <li>Sur l'onglet <b>Surveillance</b> de la page Détails de l'unité, cliquez sur <b>Gérer les superviseurs</b> sur le côté droit de la page pour gérer les moniteurs associés à ce périphérique.</li>
   <li>Sur la page Moniteurs, cliquez sur l'onglet <b>Ajouter moniteur</b>.</li>
   <li>Sélectionnez l'adresse IP à surveiller dans la liste <b>Adresse IP</b>.</li>
   <li>Sélectionnez le type de moniteur dans la liste <b>Type de moniteur</b>.</li>
   <li>Configurez les options de notification. Dans la liste <b>Avertir ?</b>, sélectionnez <b>Notifier les utilisateurs</b> pour avertir les utilisateurs de problèmes, ou <b>Ne rien faire</b> pour ignorer la notification utilisateur.</li>
   <li>Sélectionnez le délai d'envoi de la notification utilisateur dans la liste <b>Notifier attente</b>.</li>
   <li>Cliquez sur <b>Ajouter moniteur</b> afin d'ajouter le moniteur pour le périphérique. Le nouveau moniteur s'affiche dans la section <b>Editer les superviseurs existants</b> de l'écran.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Edition d'un moniteur existant</td>
   <td>
   <ol>
   <li>Sur la page Moniteurs sous l'en-tête <b>Editer les superviseurs existants</b>, cliquez sur des détails de moniteur pour ouvrir le moniteur afin de pouvoir l'éditer.</li>
   <li>Mettez à jour une des zones suivantes : Type de moniteur, Notifier, Notifier attente.</li>
   <li>Cliquez sur <b>Mettre à jour</b> pour mettre à jour les détails. Cliquez sur <b>Annuler</b> pour annuler l'édition.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Suppression d'un moniteur</td>
   <td>
   <ol>
   <li>Sur la page Moniteurs sous l'en-tête <b>Editer les superviseurs existants</b>, cliquez sur l'icône Supprimer en regard des détails du moniteur.</li>
   <li>Cliquez sur <b>Oui</b> pour retirer le moniteur. cliquez sur <b>Non</b> pour annuler l'action,</li>
   </ol>
   </td>
   </tr>
   </TBODY>
   </table>

## Etapes suivantes

- Si un nouveau moniteur est ajouté, il apparaît sur l'onglet **Surveillance**. Le moniteur envoie une demande ping au périphérique toutes les 5 minutes et s'attend à recevoir une réponse qui varie en fonction de type de demande ping sélectionné. Si la réponse attendue n'est pas reçue, un courrier électronique est envoyé à l'adresse électronique de notification pour le compte dans le délai indiqué, si l'option de notification est sélectionnée.
- Si un moniteur est édité, il continue de fonctionner comme indiqué dans les détails le concernant. Si le type est modifié, le délai d'attente pour la réception de la demande ping attendue est différent. Si les options de notification sont modifiées, la façon dont les utilisateurs sont avertis qu'une tentative a échoué change en fonction des nouvelles sélections. Le moniteur reste accessible depuis l'onglet **Surveillance**.
- Si un moniteur est retiré, il ne fonctionne plus pour le périphérique. La surveillance qui est associée au moniteur retiré s'arrête complètement et ce dernier n'apparaît plus dans l'onglet **Surveillance**.
