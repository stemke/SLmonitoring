---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestión de IBM Cloud Monitoring Service para el agente nativo IaaS (Beta)

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service para el agente nativo IaaS recopila datos de métricas del dispositivo en el que está instalado y los envía al almacenamiento de métricas. Desde el almacenamiento de métricas, los datos están disponibles para la interfaz de usuario para la supervisión simple y para Grafana para consultas avanzadas.
Si utiliza IBM Cloud Monitoring Service para el agente nativo IaaS, siga estos pasos para ver, detener, iniciar o desinstalar el servicio para el servidor.
{:shortdesc}

<table>
   <CAPTION>Tabla 1. IBM Cloud Monitoring Service para el agente nativo IaaS</CAPTION>
   <THEAD>
   <TR>
   <th>Si la acción que se va a emprender es...</th>
   <th>Entonces, para Linux...</th>
     <th>Entonces, para FreeBSD...</th>
     <th>Entonces, para Windows...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Ver el estado del servicio</td>
   <td>
   Utilice el mandato `service monitoring status`
   </td>
     <td>
   Utilice el mandato `service monitoring status`
   </td>
     <td>
   Utilice el mandato `sc.exe query monitoring`
   </td>
   </tr>
   <tr>
   <td>Detener el servicio de supervisión</td>
   <td>
   Utilice el mandato `service monitoring stop`
   </td>
     <td>
   Utilice el mandato `service monitoring stop`
   </td>
     <td>
   Utilice el mandato `sc.exe stop monitoring`
   </td>
   </tr>
       <tr>
   <td>Iniciar el servicio de supervisión</td>
   <td>
   Utilice el mandato `service monitoring start`
   </td>
     <td>
   Utilice el mandato `service monitoring start`
   </td>
     <td>
   Utilice el mandato `sc.exe start monitoring`
   </td>
   </tr>
       <tr>
   <td>Desinstalación del servicio de supervisión</td>
   <td>Escriba estos mandatos:
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>Escriba estos mandatos:
  <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>Siga estos pasos:
 <ol>
       <li>Abra **Agregar o quitar programas**.</li>
       <li>Seleccione **IBM Cloud Monitoring Agent**</li>
   <li>Pulse **Desinstalar**.</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>
