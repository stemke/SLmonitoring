---
copyright:
  years: 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gerenciando o IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)

O {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent coleta dados de métrica do dispositivo no qual está instalado e os envia para o armazenamento de métrica. No armazenamento de métrica, os dados ficam disponíveis na interface com o usuário para simples monitoramento e no Grafana para consultas avançadas.
Se você estiver usando o IBM Cloud Monitoring Service for IaaS Bare Metal Agent, siga estas etapas para visualizar, parar, iniciar ou desinstalar o serviço de seu servidor.
{:shortdesc}

<table>
   <CAPTION>Tabela 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
   <THEAD>
   <TR>
   <th>Se a ação a ser tomada é...</th>
   <th>Então, para o Linux...</th>
     <th>Então, para o FreeBSD...</th>
     <th>Então, para o Windows...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Visualizar o status do serviço</td>
   <td>
   Use o comando `service monitoring status`
   </td>
     <td>
   Use o comando `service monitoring status`
   </td>
     <td>
   Use o comando `sc.exe query monitoring`
   </td>
   </tr>
   <tr>
   <td>Parar o serviço de monitoramento</td>
   <td>
   Use o comando `service monitoring stop`
   </td>
     <td>
   Use o comando `service monitoring stop`
   </td>
     <td>
   Use o comando `sc.exe stop monitoring`
   </td>
   </tr>
       <tr>
   <td>Iniciar o serviço de monitoramento</td>
   <td>
   Use o comando `service monitoring start`
   </td>
     <td>
   Use o comando `service monitoring start`
   </td>
     <td>
   Use o comando `sc.exe start monitoring`
   </td>
   </tr>
       <tr>
   <td>Desinstalar o serviço de monitoramento</td>
   <td>Insira esses comandos:
     <ol>
       <li>`/opt/monitoring/baremetal-monitoring-agent-linux-amd64 -uninstall`</li>
       <li>`rm -rf /opt/monitoring`</li>
     </ol>
   </td>
     <td>Insira esses comandos:
  <ol>
    <li>`service monitoring stop`</li>
    <li>`rm -rf /opt/monitoring`</li>
    <li>`rm /etc/rc.d/monitoring`</li>
<li>`sysrc monitoring_enable="NO"`</li>
     </ol>
   </td>
     <td>Siga estas etapas:
 <ol>
       <li>Abra **Incluir ou remover programas**.</li>
       <li>Selecione **IBM Cloud Monitoring Agent**</li>
   <li>Clique em **Desinstalar**.</li>
     </ol>
   </td>
   </tr>
   </TBODY>
   </table>



