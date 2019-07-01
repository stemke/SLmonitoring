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

# Configurando um relatório de agente do Nimsoft Monitoring
{: #configuring-a-nimsoft-monitoring-agent-report}

## Antes
de Começar

Primeiro, navegue para o menu de dispositivos e assegure-se de ter as permissões de conta corretas para concluir as tarefas.

* Navegue para o menu de dispositivos do console. Para obter mais informações, consulte [Navegando para os dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assegure-se de que você tenha as permissões de conta e o acesso ao dispositivo necessários. Somente o proprietário da conta ou um usuário com a permissão de infraestrutura clássica **Gerenciar usuários** pode ajustar as permissões.

Para obter mais informações sobre as permissões, consulte [Permissões de infraestrutura clássica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gerenciando o acesso ao dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Configurando um relatório de agente do Nimsoft Monitoring
{: #configuring-nimsoft-monitoring-agent-report-steps}

Conclua as etapas a seguir para configurar um relatório do agente Nimsoft Monitoring.

1. No menu **Dispositivos**, selecione **Monitoramento**.
2. Na página **Monitoramento**, selecione **Configurar relatórios
do agente** no menu suspenso **Ações** na coluna **Avançado**.
3. Selecione o agente a ser configurado na lista suspensa **Agentes**.
  
  Os agentes disponíveis variam por dispositivo e são dependentes do pacote de monitoramento
aplicado ao dispositivo.
  {:note}

4. Selecione a seção a ser configurada na lista suspensa **Seções**. Se você selecionar uma seção que contém perfis, outra lista suspensa aparecerá. Nessa lista, selecione um **perfil existente** na lista suspensa **Perfis**. Para incluir uma nova configuração, selecione **Incluir configuração do agente...** na lista suspensa **Perfis**.

5. Preencha cada campo na seção **Métricas gerais e informações**, se necessário.
  
  Os campos
obrigatórios são indicados por um asterisco vermelho (*). Nem todos os agentes, seções ou perfis contêm esta seção.
  {:note}

6. Clique na caixa de seleção **Métrica** para cada métrica a ser incluída no relatório na seção **Selecionar métricas sobre as quais relatar**, se aplicável.

7. Clique na caixa de seleção **Alarme** de cada alarme a ser ativado para o Agente em **Alarmes da métrica**.

  Nem todos os alarmes nesta seção estão ligados a uma métrica específica. Os alarmes são enviados para cada endereço de e-mail associado à seção **Assinantes de alarme** do Agente.
  {:note}

7. Clique em **Salvar** para salvar a configuração. Clique em **Cancelar** para cancelar a ação.
  
  O botão **Salvar** ficará desativado até que você faça uma mudança na
configuração atual.
  {:note}

## Próximos passos

Depois que a configuração é salva com sucesso, aparece uma mensagem de confirmação. Se a configuração tiver sido malsucedida, uma mensagem de erro aparecerá com detalhes sobre o erro ocorrido e como corrigi-lo. É possível reconfigurar agentes a qualquer momento ao repetir essas etapas.
