---

copyright:
  years: 2014, 2017
lastupdated: "2017-10-30"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configurando um relatório de agente do Nimsoft Monitoring
{: #configuring-a-nimsoft-monitoring-agent-report}

1. Na tela de monitoramento, selecione **Configurar relatórios do agente** no menu suspenso **Ações** na coluna **Avançado**.

2. Selecione o agente a ser configurado na lista suspensa **Agentes**.
  * **Nota:** os agentes disponíveis variam por dispositivo e são dependentes do
pacote de monitoramento aplicado ao dispositivo.

3. Selecione a seção a ser configurada na lista suspensa **Seções**. Se você selecionar uma seção que contém perfis, outra lista suspensa aparecerá. Nessa lista, selecione um **perfil existente** na lista suspensa **Perfis**. Para incluir uma nova configuração, selecione **Incluir configuração do agente...** na lista suspensa **Perfis**.

4. Preencha cada campo na seção **Métricas gerais e informações**, se necessário.
  * **Nota:** os campos obrigatórios são indicados por um asterisco vermelho (*). Nem todos os agentes, seções ou perfis contêm esta seção.

5. Clique na caixa de seleção **Métrica** para cada métrica a ser incluída no relatório na seção **Selecionar métricas sobre as quais relatar**, se aplicável.

6. Clique na caixa de seleção **Alarme** de cada alarme a ser ativado para o Agente em **Alarmes da métrica**.
  * **Nota:** nem todos os alarmes desta seção são ligados a uma métrica específica. Os alarmes são enviados para cada endereço de e-mail associado à seção **Assinantes de alarme** do Agente.

7. Clique em **Salvar** para salvar a configuração. Clique em **Cancelar** para cancelar a ação.
  * **Nota:** o botão de salvamento fica desativado até que você faça uma mudança na configuração atual.

## Próximos passos

Depois que a configuração é salva com sucesso, aparece uma mensagem de confirmação. Se a configuração tiver sido malsucedida, uma mensagem de erro aparecerá com detalhes sobre o erro ocorrido e como corrigi-lo. É possível reconfigurar agentes a qualquer momento ao repetir essas etapas.
