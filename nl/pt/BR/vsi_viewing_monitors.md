---

copyright:
  years: 2017, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:note: .note}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Visualizando e gerenciando monitores
{: #viewing-and-managing-monitors}

Monitorar um dispositivo permite que você inicie o serviço e reduza a velocidade dos pings
para assegurar que o dispositivo esteja on-line e responsivo.
{:shortdesc}

Se um eco não for recebido no prazo atribuído (1 segundo para pings de serviço, 5 segundos para pings lentos), um alerta será enviado para o endereço
de e-mail na conta. Um status de **Ativo** no campo **Status** indica que um eco foi recebido, enquanto que **Inativo** indica que o eco não foi recebido. Se você tiver um monitor básico configurado, siga estas etapas para visualizar e gerenciar o monitoramento para um dispositivo.

## Antes
de Começar
Primeiro, navegue para o menu de dispositivos e assegure-se de ter as permissões de conta corretas para concluir as tarefas.

* Navegue para o menu de dispositivos do console. Para obter mais informações, consulte [Navegando para os dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assegure-se de que você tenha as permissões de conta e o acesso ao dispositivo necessários. Somente o proprietário da conta ou um usuário com a permissão de infraestrutura clássica **Gerenciar usuários** pode ajustar as permissões.

Para obter mais informações sobre as permissões, consulte [Permissões de infraestrutura clássica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gerenciando o acesso ao dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Visualizando monitores
{: #viewing-monitors}

1. No menu **Dispositivos**, selecione **Lista de dispositivos**.
2. Clique no nome do dispositivo para acessá-lo.
3. Clique na guia **Monitoramento**. Todos os pings atuais são visualizáveis na página de entrada.

A guia **Monitoramento** somente estará visível se, pelo menos, um monitor
estiver configurado.
{:note}

## Incluindo um monitor
{: #adding-a-monitor}

1. No menu **Dispositivos**, selecione **Lista de dispositivos**.
2. Clique no nome do dispositivo para acessá-lo.
3. Clique na guia **Monitoramento** e selecione **Gerenciar monitores**.
4. Selecione **Incluir monitor**.
5. Selecione o endereço IP a monitorar no campo **Endereço IP** e o tipo
de monitor no campo **Tipo de monitor**. 
6. Configure as opções de notificação. No campo **Notificar?**, selecione **Notificar usuários** para notificar os usuários sobre problemas ou selecione
**Não fazer nada** para efetuar bypass da notificação do usuário.
7. Selecione o intervalo de tempo para notificação do usuário no campo **Espera da notificação**.
8. Clique em **Incluir monitor** para incluir o monitor no dispositivo. O
novo monitor aparece na seção **Editar monitores existentes**.

## Editando um monitor existente
{: #editing-an-exisiting-monitor}

1. No menu **Dispositivos**, selecione **Lista de dispositivos**.
2. Clique no nome do dispositivo para acessá-lo.
3. Clique na guia **Monitoramento** e selecione **Gerenciar monitores**.
4. Na seção **Editar monitores existentes**, clique em qualquer um dos
detalhes do monitor para abrir o monitor para edições.
5. Atualize qualquer um dos campos a seguir: **Tipo de monitor, notificar,** ou **Espera da notificação**.
6. Clique em **Atualizar** para atualizar os detalhes.

## Removendo um monitor
{: #removing-a-monitor}

1. No menu **Dispositivos**, selecione **Lista de dispositivos**.
2. Clique no nome do dispositivo para acessá-lo.
3. Clique na guia **Monitoramento** e selecione **Gerenciar monitores**.
4. Na seção **Editar monitores existentes**, clique no ícone **Remover** nos detalhes do monitor.
5. Selecione **Sim** para remover o monitor.

## Próximos passos

- Se um novo monitor for incluído, ele aparecerá na guia **Monitoramento**. O monitor envia um ping para o dispositivo a cada 5 minutos, esperando uma resposta baseada no tipo de ping selecionado. Se a resposta esperada não for recebida, será enviado um e-mail para o endereço de e-mail de notificação para a conta no prazo especificado, se a opção de notificação estiver selecionada.
- Se um monitor for editado, ele continuará a funcionar conforme especificado nos detalhes. Se o tipo for mudado, a quantia esperada de tempo para receber o ping será diferente. Se as opções de notificação tiverem mudado, a maneira com que os usuários serão notificados sobre uma tentativa com falha mudará com base nas novas seleções. O monitor permanece acessível na guia **Monitoramento**.
- Se um monitor for removido, ele não funcionará mais para o dispositivo. Todo o monitoramento associado ao monitor removido parará e o monitor não aparecerá mais na guia **Monitoramento**.

