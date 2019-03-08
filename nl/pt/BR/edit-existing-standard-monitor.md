---

copyright:
  years: 2014, 2018
lastupdated: "2018-10-30"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Editando um monitor existente
Depois que um monitor é incluído em um dispositivo, é possível modificar ou removê-lo a qualquer momento. As modificações nos monitores permitem mudanças no tipo e nas opções de notificação, enquanto a remoção de um monitor cancela o monitor completamente. Siga estas etapas para editar um monitor existente.

1. Na página **Monitores** no título **Editar monitores existentes**, clique em qualquer um dos detalhes do monitor para abri-lo para edição.

2. Modifique os **Detalhes do monitor** conforme necessário. Consulte esta tabela para obter mais
detalhes sobre cada campo editável.

|Campo|Detalhes|Ação|
|---|---|---|
|Tipo de monitor|O período de tempo em que uma resposta do dispositivo é esperada. O sistema é padronizado com um ping de serviço. Um ping lento aguarda 5 segundos por uma resposta, permitindo aos servidores otimizados para tarefas que não são da rede mais tempo para processar a solicitação. Um ping de serviço emite um ping a cada 5 minutos e espera uma resposta de eco em 1 segundo. Se mais de um ping for perdido, um alerta será emitido.|Selecione entre **Ping lento** ou **Ping de serviço**.|
|Notificar| Os usuários notificados receberão notificações automatizadas sempre que um dispositivo não responder a um ping no tempo de resposta atribuído. Para receber uma notificação, um usuário deve estar na conta associada ao dispositivo.|Para incluir um usuário, selecione o novo **Usuário notificado** e clique em **Incluir usuário**. Para remover um usuário, clique no ícone **Remover** próximo ao Usuário notificado existente e clique em **Sim** para confirmar sua ação.|
|Notificar espera|O período de tempo que o sistema aguarda para enviar uma notificação quando o dispositivo não respondeu ao ping. Múltiplos tempos de espera estão disponíveis. **Nota:** os detalhes de notificação não são necessários quando não há usuários selecionados para notificação. |Selecione
o tempo de espera necessário.|

3. Clique em **Atualizar** para aplicar as mudanças ao monitor. Clique em **Cancelar** para cancelar a ação.

## Próximos passos

Se um monitor for editado, ele continuará a funcionar conforme especificado nos detalhes. Se o tipo for mudado, a quantia esperada de tempo para receber o ping será diferente. Se as opções de notificação mudarem, o modo de notificação mudará com base nas novas seleções. O monitor permanece acessível na guia de monitoramento.
