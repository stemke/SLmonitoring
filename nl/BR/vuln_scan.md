---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Varreduras de vulnerabilidade
Parceiros do {{site.data.keyword.BluSoftlayer_full}} com o Nessus para fornecer varreduras de vulnerabilidade para qualquer dispositivo na rede do {{site.data.keyword.BluSoftlayer_notm}}. As varreduras de vulnerabilidade testam áreas de fraqueza em um dispositivo e retornam um relatório da análise, dos problemas de segurança e das correções para seu dispositivo host. A execução de varreduras de vulnerabilidade nos dispositivos assegura que eles fiquem sempre seguros e também sejam o primeiro recurso a ser empregado quando você acha que um dispositivo pode estar vulnerável ou comprometido. As varreduras de vulnerabilidade podem ser concluídas usando o [Portal do cliente ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/) em qualquer dispositivo associado à sua conta.
{:shortdesc}

## Nessus Security Scanner 
O {{site.data.keyword.BluSoftlayer_notm}} fornece um scanner de segurança on-line, desenvolvido com a ferramenta de software livre Nessus Scanning. Esse scanner de segurança pode ser acessado na guia Segurança clicando em **Scanner**. Para obter mais informações, veja [ferramenta Nessus Scanning ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://www.nessus.org/nessus/).

A página **Scanner** fornece uma lista de hardware disponível para a ferramenta Nessus hospedada pelo {{site.data.keyword.BluSoftlayer_notm}}. Para varrer um servidor ou para ver os resultados de uma varredura anterior, clique no link de detalhes do servidor que você deseja inspecionar. A página de detalhes de varredura de vulnerabilidade mostra um breve resumo do servidor (contendo o nome do servidor, o endereço IP a ser varrido e o data center no qual o servidor está localizado.) **Iniciar varredura** planeja seu servidor com o servidor de varredura Nessus para ser varrido quanto à vulnerabilidade assim que possível.

Após o resumo do servidor, há uma tabela de varreduras de vulnerabilidade atuais e passadas do Nessus. Listados para cada varredura estão a data de solicitação da varredura, a data de início da varredura, o status da varredura e, se a varredura tiver sido concluída, um link para o relatório Nessus.

Os relatórios do Nessus podem ter um destes status:

* Varredura pendente: a varredura foi planejada para a caixa do scanner Nessus.
* Varredura em processamento: a varredura está atualmente em andamento.
* Gerando relatório: a varredura foi concluída e os resultados do teste estão sendo compilados em um relatório.
* Varredura completa: a varredura foi concluída com sucesso e o relatório de vulnerabilidade foi gerado.
* Varredura cancelada: a varredura Nessus foi cancelada manualmente por um técnico do {{site.data.keyword.BluSoftlayer_notm}}.

Para obter todas as varreduras do Nessus concluídas com sucesso listadas nesta tabela, um relatório pode ser visualizado clicando em **Visualizar relatório**. O relatório possui duas tabelas: uma tabela Detalhes da varredura, que lista o número de hosts que foram varridos, o número de vulnerabilidades de segurança abertas (buracos) localizadas e o número de possíveis vulnerabilidades de segurança (avisos) localizadas. A segunda tabela lista todos os problemas de segurança localizados: o host no qual a vulnerabilidade foi localizada e uma descrição da possível vulnerabilidade.

A ferramenta de software livre Nessus se baseia em plug-in, que permite que novos testes sejam desenvolvidos conforme as vulnerabilidades são localizadas. O {{site.data.keyword.BluSoftlayer_notm}} atualiza a ferramenta Nessus interna regularmente, portanto, a varredura regular com o scanner de segurança é recomendada para manter atualizado com novas ameaças.

Para que a varredura seja bem-sucedida, as conexões de 173.192.255.232 e 172.17.19.38 precisam ter o acesso permitido ao servidor.
