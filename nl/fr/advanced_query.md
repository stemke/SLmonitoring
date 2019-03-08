---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Création d'une requête de surveillance avancée (Bêta)

Dans {{site.data.keyword.cloud}}, vous pouvez utiliser Grafana, une plateforme d'analyse et de visualisation open source, pour surveiller, rechercher, analyser et visualiser vos métriques dans une grande variété de graphiques, tels que des diagrammes et des tableaux. Vous pouvez utiliser Grafana pour effectuer des tâches d'analyse avancées.
{:shortdesc}

Si vous utilisez Grafana, vous pouvez utiliser le tableau de bord pour créer des graphiques à l'aide de la requête de métrique.
1. [Accédez au tableau de bord Grafana](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-navigating_grafana#navigating_grafana).
2. Sélectionnez le domaine `account` et un compte utilisateur avec un IBMid lié au périphérique bare metal.
3. Utilisez le format suivant pour créer vos requêtes :
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. Les types de métrique disponibles sont les suivants :
<table>
   <CAPTION>Tableau 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Type</th>
     <th>Unités</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>octets</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>octets</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>octets</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>octets</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>octets/seconde</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>octets/seconde</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>opérations/seconde</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>opérations/seconde</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>temps d'attente en millisecondes par opération</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>temps d'attente en millisecondes par opération</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` or `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>octets/seconde</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` or `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>octets/seconde</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` ou `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>nombre</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` ou `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>nombre</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` ou `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>nombre</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` ou `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>nombre</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>Cette métrique n'est pas disponible pour tous les périphériques. </td>
       <td>degrés Celsius</td>
     </tr>
   </TBODY>
   </table>

Pour plus d'informations, voir [Configuration d'une requête de métrique dans Grafana](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-define_query#define_query).
