---
copyright:
  years: 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestion d'IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Bêta)

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent collecte des données de métrique à partir du périphérique sur lequel il est installé et envoie ces données à l'espace de stockage des métriques. A partir de l'espace de stockage des métriques, les données sont disponibles sur l'interface utilisateur pour la surveillance simple et sur Grafana pour les requêtes avancées.
Si vous utilisez IBM Cloud Monitoring Service for IaaS Bare Metal Agent, procédez comme indiqué ci-après afin d'afficher, d'arrêter, de démarrer ou de désinstaller le service pour votre serveur.
{:shortdesc}

<table>
   <CAPTION>Tableau 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Action</th>
   <th>Procédure pour Linux</th>
     <th>Procédure pour FreeBSD</th>
     <th>Procédure pour Windows</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Afficher l'état du service</td>
   <td>
   Utilisez la commande `service monitoring status`
   </td>
     <td>
   Utilisez la commande `service monitoring status`
   </td>
     <td>
   Utilisez la commande `sc.exe query monitoring`
   </td>
   </tr>
   <tr>
   <td>Arrêter le service de surveillance</td>
   <td>
   Utilisez la commande `service monitoring stop`
   </td>
     <td>
   Utilisez la commande `service monitoring stop`
   </td>
     <td>
   Utilisez la commande `sc.exe stop monitoring`
   </td>
   </tr>
       <tr>
   <td>Démarrer le service de surveillance</td>
   <td>
   Utilisez la commande `service monitoring start`
   </td>
     <td>
   Utilisez la commande `service monitoring start`
   </td>
     <td>
   Utilisez la commande `sc.exe start monitoring`
   </td>
   </tr>
       <tr>
   <td>Désinstaller le service de surveillance</td>
   <td>Entrez les commandes suivantes :
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>Entrez les commandes suivantes :
     <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>Procédez comme suit :
 <ol>
       <li>Sélectionnez **Ajout/Suppression de programmes**</li>
       <li>Sélectionnez **IBM Cloud Monitoring Agent**</li>
   <li>Cliquez sur **Désinstaller**</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>



