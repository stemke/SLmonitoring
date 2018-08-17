---
copyright:
  years: 1994, 2017
lastupdated: "2017-06-09"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Incluindo e removendo monitores

<table>
   <CAPTION>Tabela 1. Incluindo e removendo monitores de dispositivo</CAPTION>
   <THEAD>
   <TR>
   <th>Se a ação a ser tomada é...</th>
   <th>Então...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Incluir um monitor</td>
   <td>
   <ol>
   <li>Na guia <b>Monitoramento</b> da página Detalhes do dispositivo, clique em <b>Gerenciar monitores</b> no lado direito da página para gerenciar os monitores associados a esse dispositivo.</li>
   <li>Na página Monitores, clique na guia <b>Incluir monitor</b>.
   * **Nota:** os endereços IP Públicos e Privados estão disponíveis para monitoramento. Cada endereço IP é identificado na guia **Informações do servidor**.</li>
   <li>Selecione o endereço IP a ser monitorado na lista suspensa <b>Endereço IP</b>.</li>
   <li>Selecione o tipo de monitor na lista suspensa <b>Tipo de monitor</b>.</li>
   <li>Configure as opções de notificação. Na lista suspensa <b>Notificar?</b>, selecione <b>Notificar usuários</b> para notificar os usuários sobre problemas ou <b>Fazer nada</b> para ignorar a notificação do usuário.</li>
   <li>Selecione o prazo para notificação do usuário sobre o uso da lista suspensa <b>Notificar espera</b>.</li>
   <li>Clique em <b>Incluir monitor</b> para incluir o monitor para o dispositivo. O novo monitor aparece na seção <b>Editar monitores existentes</b> da tela.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Remover um monitor</td>
   <td>
   <ol>
   <li>Na página Monitores sob o título <b>Editar monitores existentes</b>, clique no ícone Remover próximo aos detalhes do monitor.</li>
   <li>Clique em <b>Sim</b> para remover o monitor. Clique em <b>Não</b> para cancelar a ação.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
   </table>


## Próximos passos

- Se um novo monitor for incluído, ele aparecerá na guia **Monitoramento**. O monitor envia um ping para o dispositivo a cada 5 minutos, esperando uma resposta baseada no tipo de ping selecionado. Se a resposta esperada não for recebida, será enviado um e-mail para o endereço de e-mail de notificação para a conta no prazo especificado, se a opção de notificação estiver selecionada.

- Se um monitor for removido, o monitor não funcionará mais para o dispositivo. Todo o monitoramento associado ao monitor removido cessará e o monitor não aparecerá mais na guia Monitoramento.
