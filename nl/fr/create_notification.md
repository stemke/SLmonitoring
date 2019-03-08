---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Création et gestion de notifications de moniteur (Bêta)
Une notification décrit la méthode et les détails qui sont utilisés pour envoyer une notification lorsqu'une alerte est déclenchée. Par exemple, afin d'obtenir une notification d'avertissement et une notification d'erreur pour une métrique, définissez une règle qui surveille le seuil d'avertissement et une règle qui surveille le seuil d'erreur.
{:shortdesc}

## Création d'une notification

 1. Après avoir rejoint le programme bêta, sélectionnez **Unités -> Surveillance**.
 2. Cliquez sur l'onglet **Notifications**.
 3. Cliquez sur **Créer une notification**.
 4. Entrez les informations relatives à votre nouvelle notification.

<table>
  <caption>Détails de notification par courrier électronique</caption>
  <tr>
     <th>Zone</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Identificateur unique de la notification. Cette zone est obligatoire.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Sélectionnez **Email**</td>
  </tr>
  <tr>
    <td>Email Address</td>
    <td>Entrez l'adresse électronique du destinataire.</td>
  </tr>
</table>

<table>
  <caption>Détails de notification de webhook</caption>
  <tr>
     <th>Zone</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Identificateur unique de la notification. Cette zone est obligatoire.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Sélectionnez **Webhook**</td>
  </tr>
  <tr>
    <td>Webhook URL</td>
    <td>Entrez l'URL où la demande POST doit être effectuée.</td>
  </tr>
  <tr>
  <td>Verify certificates</td>
    <td>Sélectionnez cette option pour vérifier les certificats.</td>
  </tr>
  <tr>
    <td>Webhook headers</td>
    <td>Entrez les éventuels en-têtes.</td>
  </tr>
  <tr>
    <td>Webhook query parameters</td>
    <td>Entrez les éventuels paramètres de requête.</td>
  </tr>
</table>

<table>
  <caption>Détails de notification Pager duty</caption>
  <tr>
     <th>Zone</th>
     <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Identificateur unique de la notification. Cette zone est obligatoire.</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>Sélectionnez **Pager duty**</td>
  </tr>
  <tr>
    <td>API Key</td>
    <td>Entrez la clé d'API pour les notifications Pager duty.</td>
  </tr>
</table>


5. Cliquez sur **Ok** pour créer les nouvelles notifications avec le paramètre que vous avez spécifié. 

## Edition d'une notification
 1. Après avoir rejoint le programme bêta, sélectionnez **Unités -> Surveillance**.
 2. Cliquez sur l'onglet **Notifications**.
3. Cliquez sur **Actions->Editer une notification**.
4. Editez n'importe lequel des détails de notification.
5. Cliquez sur **Ok** pour accepter vos modifications.

## Suppression d'une notification
1. Après avoir rejoint le programme bêta, sélectionnez **Unités -> Surveillance**.
2. Cliquez sur l'onglet **Notifications**.
3. Cliquez sur **Actions->Supprimer une notification**.
4. Cliquez sur **Supprimer** pour confirmer la suppression.

## Ajout de plusieurs notifications à un périphérique
1. Sélectionnez **Infrastructure->Liste des unités->*Nom d'unité*** pour accéder aux détails du périphérique.
2. Cliquez sur **Actions->Gérer les notifications**.
4. Cliquez pour affecter ou retirer des notifications pour votre périphérique.
