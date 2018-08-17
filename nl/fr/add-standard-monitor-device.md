---
copyright:
  years: 1994, 2017
lastupdated: "2017-06-09"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Ajout et retrait de moniteurs

<table>
   <CAPTION>Tableau 1. Affichage et retrait de moniteurs de périphérique</CAPTION>
   <THEAD>
   <TR>
   <th>Action</th>
   <th>Procédure</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Ajout d'un moniteur</td>
   <td>
   <ol>
   <li>Sur l'onglet <b>Surveillance</b> de la page Détails de l'unité, cliquez sur <b>Gérer les superviseurs</b> sur le côté droit de la page pour gérer les moniteurs qui sont associés à ce périphérique. </li>
   <li>Sur la page Moniteurs, cliquez sur l'onglet <b>Ajouter moniteur</b>.
   * **Remarque :** des adresses IP publiques et privées sont disponibles pour la surveillance. Chaque adresse IP est identifiée sur l'onglet **Info Serveur**. </li>
   <li>Sélectionnez l'adresse IP à surveiller dans la liste déroulante <b>Adresse IP</b>.</li>
   <li>Sélectionnez le type de moniteur dans la liste déroulante <b>Type de moniteur</b>.</li>
   <li>Configurez les options de notification. Dans la liste <b>Avertir ?</b>, sélectionnez <b>Notifier les utilisateurs</b> pour avertir les utilisateurs de problèmes, ou <b>Ne rien faire</b> pour ignorer la notification utilisateur. </li>
   <li>Sélectionnez le délai d'envoi de notification utilisateur dans la liste déroulante <b>Notifier attente</b>.</li>
   <li>Cliquez sur <b>Ajouter moniteur</b> afin d'ajouter le moniteur pour le périphérique. Le nouveau moniteur s'affiche dans la section <b>Editer les superviseurs existants</b> de l'écran.</li>
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

- Si un moniteur est supprimé, ce dernier ne fonctionne plus pour le périphérique. La surveillance qui est associée au moniteur retiré s'arrête complètement et ce dernier n'apparaît plus dans l'onglet Surveillance. 
