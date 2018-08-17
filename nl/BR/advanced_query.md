---
copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Criando uma consulta de monitoramento avançada (Beta)

No {{site.data.keyword.cloud}}, é possível usar o Grafana, uma plataforma de software livre para análise e visualização, para monitorar, procurar, analisar e visualizar suas métricas em uma variedade de gráficos, por exemplo, gráficos e tabelas. É possível usar o Grafana para executar tarefas analíticas avançadas.
{:shortdesc}

Se você usar o Grafana, será possível usar o painel para criar gráficos usando a consulta de métrica.
1. [Navegue para o painel do Grafana](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/navigating_grafana.html#navigating_grafana).
2. Selecione o domínio `account` e uma conta do usuário com um IBMid vinculado ao dispositivo bare metal. 
3. Use esse formato para criar suas consultas.
`ibmcloud.public.iaas-telemetry.region.<DATACENTER_BAREMETAL_LIVES_IN>.<MACHINE_GUID>.<METRIC_TYPE>`
4. Aqui estão os tipos de métricas disponíveis:
<table>
   <CAPTION>Tabela 1. IBM Cloud Monitoring Service for IaaS Bare Metal Agent</CAPTION>
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
       <td>operações/segundo</td>
     </tr>
      <tr>
       <td>`disk-write-iops-<id>`<br>`disk-write-iops-agg`</td>
       <td>operações/segundo</td>
     </tr>
     <tr>
       <td>`disk-read-latency-<id>`<br>`disk-read-latency-avg`</td>
       <td>Latência em milissegundos por operação</td>
     </tr>
    <tr>
       <td>`disk-write-latency-<id>`<br>`disk-write-latency-avg`</td>
       <td>Latência em milissegundos por operação</td>
     </tr>
     <tr>
       <td>`net-public-in-bps-<id>`<br>`net-public-in-bps-agg` ou `net-private-in-bps-<id>
net-private-in-bps-agg`</td>
       <td>bytes/segundo</td>
     </tr>
      <tr>
       <td>`net-public-out-bps-<id>`<br>`net-public-out-bps-agg` ou `net-private-out-bps-<id>
net-private-out-bps-agg`</td>
       <td>bytes/segundo</td>
     </tr>
     <tr>
       <td>`net-public-in-packets-<id>`<br>`net-public-in-packets-agg` ou `net-private-in-packets-<id> net-private-in-packets-agg`</td>
       <td>número</td>
     </tr>
   <tr>
       <td>`net-public-out-packets-<id>`<br>`net-public-out-packets-agg` ou `net-private-out-packets-<id> net-private-out-packets-agg`</td>
       <td>número</td>
     </tr>
   <tr>
       <td>`net-public-in-errors-<id>` <br>`net-public-in-errors-agg` ou `net-private-in-errors-<id> net-private-in-errors-agg`</td>
       <td>número</td>
     </tr>
      <tr>
       <td>`net-public-out-errors-<id>` <br>`net-public-out-errors-agg` ou `net-private-out-errors-<id> net-private-out-errors-agg`</td>
       <td>número</td>
     </tr>
    <tr>
       <td>`temperature-celsius-<id>` <br>`temperature-celsius-avg`
         <br>Essa métrica não está disponível para todos os dispositivos.</td>
       <td>graus Celsius</td>
     </tr>
   </TBODY>
   </table>

Para obter mais informações, veja [Configurando uma consulta de métrica no Grafana](https://console.bluemix.net/docs/services/cloud-monitoring/grafana/define_query.html#define_query).
