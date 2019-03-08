---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# Introdução ao IBM Cloud Monitoring (Beta)
{: #gettingstartedbeta}

Este aplicativo de monitoramento beta, construído no {{site.data.keyword.BluSoftlayer_full}} Monitoring Service, está disponível para servidores virtuais e bare metal. Para obter atualizações no desenvolvimento desse programa Beta, veja o [Blog do IBM Cloud ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}.
{:shortdesc}

## Pré-requisitos

Para participar desse programa Beta, deve-se atender a estes requisitos.
1. Sua conta do SoftLayer deve ser vinculada a uma conta do IBM Cloud com autenticação IBMid. Para vincular uma conta, o usuário principal em sua conta do SoftLayer deve efetuar login no [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com){: new_window} e no menu **Conta**, clicar em **Vincular uma conta do Bluemix**.
2. Cada usuário que visualizará o Beta deve ser vinculado a um IBMid. Para obter mais informações, veja [Vinculando contas do usuário IBMid](/docs/account?topic=account-unifyingaccounts#link_customer_accounts).
3. Cada usuário que visualizará o Beta deve ter acesso ao IBM Cloud Monitoring Service.
   1. No console do [IBM Cloud ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://console.bluemix.net){: new_window},  selecione **Gerenciar -> Conta -> Usuários**.
   2. Convide o usuário para a conta ou selecione o usuário na lista.
   3. Selecione **Designar acesso aos recursos** para o usuário.
   4. Em **Serviço**, selecione **IBM Cloud Monitoring Service**.
   5. Selecione a **Função** a ser concedida ao usuário para todas as regiões.

Se você não atender a esses pré-requisitos, não conseguirá acessar o monitoramento Beta neste momento.


## Associando-se ao beta

Siga estas etapas para iniciar o monitoramento do programa Beta. Associar-se ao Beta ativa o serviço para todos os servidores virtuais e bare metal elegíveis em sua conta. Clicar em associar não afeta o monitoramento ou os dados Nimsoft existentes.
1. (Bare metal somente) [Instale o agente de monitoramento em seu servidor bare metal](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-).
<table>
   <CAPTION>Tabela 1. Escolher um log no local</CAPTION>
   <THEAD>
   <TR>
   <th>Se desejar associar-se ao...</th>
   <th>Então...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Catálogo do IBM Cloud</td>
   <td>
   <ol>
   <li>Abra uma nova janela do navegador e insira <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>.</li>
   <li>Clique no link <b>Efetuar login</b>. </li>
   <li>Insira seu e-mail ou IBMid e clique em <b>Continuar</b>.</li>
   <li>Insira sua senha e clique em <b>Efetuar login</b>.</li>
   <li>Selecione **Infraestrutura->Lista de dispositivo->*Nome do dispositivo*** para acessar os detalhes do dispositivo.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Portal do Cliente</td>
   <td>
   <ol>
   <li>Abra uma nova janela do navegador e insira <a href="https://control.softlayer.com">https://control.softlayer.com</a>.</li>
   <li>Digite seu nome de usuário e senha e clique em <b>Efetuar login</b>. Ou clique em <b>Efetuar login com o IBMid</b>. Em seguida, insira seu e-mail ou IBMid e clique em <b>Continuar</b>. Insira sua senha e clique em <b>Efetuar login</b>. A página principal do {{site.data.keyword.slportal}} é aberta.</li>
     <li>Em **Dispositivos**, clique no **Nome do dispositivo** para acessar os detalhes do dispositivo.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. Selecione **Dispositivos -> Monitoramento**. Clique em **Associar-se ao beta** para visualizar as guias beta de políticas do sistema e de notificações.

## Próximos passos
1. Revise os detalhes de [métricas](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-) coletadas.
2. [Criar ou gerenciar](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-) uma notificação de monitor.
3. [Criar ou gerenciar](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-) uma política do sistema.
4. [Visualizar alertas](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-).
5. Revise os dados gráficos de monitoramento Beta disponíveis atualmente para um dispositivo selecionado.

|              Métricas                                      |  Descrição                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|Utilização da CPU                                            |   Visualize a % de utilização da CPU de cada núcleo e uma média nos núcleos. Clique em cada métrica na chave para ativar ou desativar os dados no gráfico.
|Rede Pública                                             |   Visualize os dados de entrada e saída de sua rede pública. Clique em cada métrica na chave para ativar ou desativar os dados no gráfico.       |
|Rede privada                                            |   Visualize os dados de entrada e saída de sua rede privada. Clique em cada métrica na chave para ativar ou desativar os dados no gráfico.           |
|Utilização de memória    | Visualize a % de utilização de memória de seu servidor     |
|Uso do disco    | Visualize a quantia média de dados que estão sendo lidos ou gravados do disco ou no disco, em bytes, ou a latência de disco. Clique em cada métrica na chave para ativar ou desativar os dados no gráfico.    |
|Temperatura                                                 |Visualize a temperatura de seu dispositivo bare metal em graus Celsius. Esses dados não estão disponíveis para todos os dispositivos.
{: caption="Tabela 1. Métricas de Beta" caption-side="top"}   

## Limitações
Se um dispositivo for excluído, as políticas de monitoramento associadas não serão excluídas. Esteja ciente de que deve excluir manualmente o dispositivo para essas políticas.

Os dados de métrica estão disponíveis por 15 dias somente.

Podem existir somente 10 políticas de monitoramento por vez. Entretanto, uma política pode ser aplicada a múltiplos dispositivos.

## Resolução de problemas
Para visualizar algumas métricas, como utilização de memória, as ferramentas Xen são necessárias em seu servidor. Para obter informações sobre a instalação das ferramentas Xen, consulte [Preparando e importando imagens](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images).

## Feedback
Para fornecer feedback sobre esse Beta, selecione **Dispositivos -> Monitoramento** ou a página de detalhes do dispositivo e clique em **Sair do feedback** para concluir uma pesquisa de opinião curta. Para deixar o Beta e retornar para a visualização padrão, clique no link **Deixar o Beta** na parte inferior da página **Dispositivos -> Monitoramento**.
