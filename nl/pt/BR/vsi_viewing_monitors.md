---

copyright:
  years: 2017
lastupdated: "2017-09-28"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Visualizando e gerenciando monitores
{: viewing-and-managing-monitors}

Monitorar um dispositivo permite que os usuários iniciem o serviço e diminuam os pings para assegurar
que o dispositivo esteja on-line e responsivo.
{:shortdesc}

Se um eco não for recebido no prazo atribuído (1 segundo para pings de serviço, 5 segundos para pings lentos), um alerta será enviado para o endereço
de e-mail na conta. Um status de **Ativo** no campo **Status** indica que um eco foi recebido, enquanto que **Inativo** indica que o eco não foi recebido. Se você tiver um monitor básico configurado, siga estas etapas para visualizar e gerenciar o monitoramento para um dispositivo.

   <table>
   <CAPTION>Tabela 1. Visualizar e gerenciar o monitoramento de dispositivo</CAPTION>
   <THEAD>
   <TR>
   <th>Se a ação a ser tomada é...</th>
   <th>Então...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Visualizar monitores</td>
   <td>
   <ol>
   <li>Na Lista de dispositivos, clique no <b>Nome do dispositivo</b> para acessar o dispositivo.</li>
   <li>Clique na guia <b>Monitoramento</b>. Todos os pings atuais são visualizáveis na página de entrada. (A guia <b>Monitoramento</b> estará visível somente se pelo menos um monitor estiver configurado.)</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Incluir um monitor</td>
   <td>
   <ol>
   <li>Na guia <b>Monitoramento</b> da página Detalhes do dispositivo, clique em <b>Gerenciar monitores</b> no lado direito da página para gerenciar os monitores associados a esse dispositivo.</li>
   <li>Na página Monitores, clique na guia <b>Incluir monitor</b>.</li>
   <li>Selecione o endereço IP a ser monitorado na lista <b>Endereço IP</b>.</li>
   <li>Selecione o tipo de monitor na lista <b>Tipo de monitor</b>.</li>
   <li>Configure as opções de notificação. Na lista <b>Notificar?</b> , selecione <b>Notificar usuários</b> para notificar os usuários sobre problemas ou <b>Não fazer nada</b> para ignorar a notificação do usuário.</li>
   <li>Selecione o prazo para notificação do usuário na lista de uso <b>Notificar espera</b>.</li>
   <li>Clique em <b>Incluir monitor</b> para incluir o monitor para o dispositivo. O novo monitor aparece na seção <b>Editar monitores existentes</b> da tela.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Edite um monitor existente</td>
   <td>
   <ol>
   <li>Na página Monitores sob o título <b>Editar monitores existentes</b>, clique em qualquer um dos detalhes do monitor para abrir o monitor para edições.</li>
   <li>Atualize qualquer um dos campos a seguir: Tipo de monitor, Notificar, Notificar espera.</li>
   <li>Clique em <b>Atualizar</b> para atualizar os detalhes. Clique em <b>Cancelar</b> para cancelar a edição.</li>
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
- Se um monitor for editado, ele continuará a funcionar conforme especificado nos detalhes. Se o tipo for mudado, a quantia esperada de tempo para receber o ping será diferente. Se as opções de notificação tiverem mudado, a maneira com que os usuários serão notificados sobre uma tentativa com falha mudará com base nas novas seleções. O monitor permanece acessível na guia **Monitoramento**.
- Se um monitor for removido, ele não funcionará mais para o dispositivo. Todo o monitoramento associado ao monitor removido parará e o monitor não aparecerá mais na guia **Monitoramento**.
