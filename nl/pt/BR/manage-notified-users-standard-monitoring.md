---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gerenciando usuários notificados para o monitoramento padrão
{: #managing-notified-users-for-standard-monitoring}

Os usuários notificados para o serviço de monitoramento padrão receberão notificações automatizadas sempre que um dispositivo não responder a um ping no tempo de resposta atribuído. É possível incluir ou remover usuários notificados a qualquer momento e os usuários notificados deverão estar na conta associada ao dispositivo para receber uma notificação. Siga estas etapas para gerenciar usuários notificados para o serviço de monitoramento padrão.
{:shortdesc}

## Antes
de Começar
Primeiro, navegue para o menu de dispositivos e assegure-se de ter as permissões de conta corretas para concluir as tarefas.

* Navegue para o menu de dispositivos do console. Para obter mais informações, consulte [Navegando para os dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Assegure-se de que você tenha as permissões de conta e o acesso ao dispositivo necessários. Somente o proprietário da conta ou um usuário com a permissão de infraestrutura clássica **Gerenciar usuários** pode ajustar as permissões.

Para obter mais informações sobre as permissões, consulte [Permissões de infraestrutura clássica](/docs/iam?topic=iam-infrapermission#infrapermission) e [Gerenciando o acesso ao dispositivo](/docs/vsi?topic=virtual-servers-managing-device-access).

## Incluindo usuários notificados
{: #adding-notified-users}

Conclua as etapas a seguir para incluir usuários notificados para o serviço de monitoramento padrão.
1. No menu **Dispositivo**, selecione **Lista de dispositivos**.
2. Clique no nome do dispositivo para acessá-lo.
3. Clique na guia **Monitoramento** e selecione **Gerenciar monitores**.
4. Selecione **Gerenciar usuários notificados**.
5. Na lista suspensa **Usuários a notificar**, selecione o novo usuário a ser notificado.
6. Selecione **Incluir usuário**.

## Removendo usuários notificados
{: #removing-notified-users}

Conclua as etapas a seguir para remover os usuários notificados para o serviço de monitoramento padrão.
1. No menu **Dispositivo**, selecione **Lista de dispositivos**.
2. Clique no nome do dispositivo para acessá-lo.
3. Clique na guia **Monitoramento** e selecione **Gerenciar monitores**.
4. Selecione **Gerenciar usuários notificados**.
5. Clique no ícone **Remover** para remover o usuário notificado existente
e, em seguida, selecione **Sim** para remover o usuário. 

## Próximos passos

Se você incluir um usuário notificado, o usuário será notificado no caso de uma resposta de ping ausente. Se você removeu um usuário notificado, o usuário não receberá mais uma notificação referente a uma resposta perdida
de ping associada ao dispositivo.
