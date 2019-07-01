---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualizando um relatório do agente para o Nimsoft Monitoring
{: #viewing-an-agent-report-for-nimsoft-monitoring}

Os detalhes de monitoramento para o Nimsoft Monitoring estão disponíveis em relatórios do agente, que fornecem os detalhes específicos de como o agente foi configurado. 
{:shortdesc}

## Antes
de Começar
Primeiro, navegue para o menu de dispositivos e assegure-se de ter as permissões de conta corretas para concluir as tarefas.

* Navegue para o menu de dispositivos do console. Para obter mais informações, consulte [Navegando para os dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assegure-se de que você tenha as permissões de conta e o acesso ao dispositivo necessários. Somente o proprietário da conta ou um usuário com a permissão de infraestrutura clássica **Gerenciar usuários** pode ajustar as permissões.

Para obter mais informações sobre as permissões, consulte [Permissões de infraestrutura clássica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gerenciando o acesso ao dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Visualizando um relatório do agente para o Nimsoft Monitoring
{: #viewing-agent-report-nimsoft-monitoring-steps}

Conclua as etapas a seguir para visualizar um relatório do agente para o Nimsoft Monitoring.

1. Na página **Monitoramento**, selecione **Visualizar relatórios
do agente** no menu **Ações**.
2. Selecione o agente a ser visualizado na lista **Agentes**.

  Os agentes disponíveis variam por dispositivo e são dependentes do pacote de monitoramento
aplicado ao dispositivo.
  {:note}
  
3. Conclua todas as seções restantes, incluindo uma ou mais das ações a seguir:

  Cada agente varia e não inclui cada seção ou métrica. As opções disponíveis nessa tela dependem das opções de configuração disponíveis para cada agente.
  {:note}
  
  * Selecione o relatório de seção na lista **Seções**.
  * Selecione o período para o relatório na lista **Visualizar por**.
  * Clique na caixa de seleção de cada métrica que você deseja relatar na seção **Selecionar métricas sobre as quais relatar:**.
    
    Somente métricas semelhantes aparecem no mesmo gráfico. Se métricas conflitantes forem escolhidas, ocorrerá um erro após a solicitação do gráfico.
    {:note}
4. Clique em **Desenhar gráfico** para desenhar o gráfico.

## Próximos passos

Depois de desenhar o gráfico para o relatório do agente, o gráfico poderá ser redesenhado a qualquer momento para visualizar diferentes métricas ao repetir essas etapas. Não
há limite para o número de relatórios do agente que podem ser gerados dentro de um prazo configurado.
