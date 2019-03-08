---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creación de una consulta de supervisión avanzada (Beta)

En {{site.data.keyword.cloud}}, puede utilizar Grafana, una plataforma de análisis y visualización de código abierto, para supervisar, buscar, analizar y visualizar las métricas en diversos gráficos, por ejemplo, diagramas y tablas. Puede utilizar Grafana para realizar tareas analíticas avanzadas.
{:shortdesc}

Si utiliza Grafana, puede utilizar el panel de control para crear gráficos utilizando la consulta de métrica.
1. [Vaya al panel de control de Grafana](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-navigating_grafana#navigating_grafana).
2. Seleccione el dominio `account` y una cuenta de usuario con un IBMid enlazado al dispositivo nativo.
3. Utilice este formato para crear las consultas.
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. Estos son los tipos de métricas disponibles:
<table>
   <CAPTION>Tabla 1. IBM Cloud Monitoring Service para el agente nativo IaaS</CAPTION>
   <THEAD>
   <TR>
   <th>Tipo</th>
     <th>Unidades</th>
   </TR>
   </THEAD>
   <TBODY>
     <tr>
       <td>`cpu-pct-<id>`<br>`cpu-pct-avg`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-used-bytes`</td>
       <td>bytes</td>
     </tr>
   <tr>
       <td>`memory-used-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`memory-swap-bytes`</td>
       <td>bytes</td>
     </tr>
     <tr>
       <td>`memory-swap-percent`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-total-bytes-<id>` <br>`disk-total-bytes-agg`</td>
       <td>bytes</td>
     </tr>
     <tr>
       <td>`disk-used-bytes-<id>` <br>`disk-used-bytes-agg`</td>
       <td>bytes</td>
     </tr>
   <tr>
       <td>`disk-used-percent-<id>`</td>
       <td>%</td>
     </tr>
     <tr>
       <td>`disk-read-bps-<id>` <br>`disk-read-bps-agg`</td>
       <td>bytes/segundo</td>
     </tr>
     <tr>
       <td>`disk-write-bps-<id>`<br>`disk-write-bps-agg`</td>
       <td>bytes/segundo</td>
     </tr>
     <tr>
       <td>`disk-read-iops-<id>`<br>`disk-read-iops-agg`</td>
       <td>operaciones/segundo</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>operaciones/segundo</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>latencia en milisegundos por operación</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>latencia en milisegundos por operación</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` o `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>bytes/segundo</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` o `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>bytes/segundo</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` o `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>número</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` o `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>número</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` o `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>número</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` o `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>número</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>Esta métrica no está disponible para todos los dispositivos.</td>
       <td>grados Celsius</td>
     </tr>
   </TBODY>
   </table>

Para obtener más información, consulte [Configuración de una consulta métrica en Grafana](/docs/services/cloud-monitoring/grafana?topic=services/cloud-monitoring-define_query#define_query).
