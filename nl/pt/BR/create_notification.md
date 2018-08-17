---
copyright:
  years: 2018
lastupdated: "2018-05-18"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Criando e gerenciando as notificações do monitor (Beta)
Uma notificação descreve o método e os detalhes usados para notificar quando um alerta é acionado. Por exemplo, para obter uma notificação de aviso e uma notificação de erro para uma métrica, defina uma regra que monitore o limite de aviso e defina uma regra que monitore o limite de erro.
{:shortdesc} 

## Criar uma notificação
 
 1. Depois de instalar a versão beta, selecione **Dispositivos -> Monitoramento**. 
 2. Clique na guia **Notificações**.
 3. Clique em **Criar notificação**.
 4. Insira as informações para sua nova notificação. 

<table>
  <caption>Detalhes de notificação por e-mail</caption>
  <tr>
     <th>Campo</th>
     <th>Descrição</th>
  </tr>
  <tr>
    <td>Nome</td>
    <td>Um identificador exclusivo da notificação. Esse campo é obrigatório.</td>
  </tr>
  <tr>
    <td>Tipo</td>
    <td>Selecione: **E-mail**</td>
  </tr>
  <tr>
    <td>Endereço de email</td>
    <td>Insira o endereço de e-mail do destinatário.</td>
  </tr>
</table>

<table>
  <caption>Detalhes de notificação do webhook</caption>
  <tr>
     <th>Campo</th>
     <th>Descrição</th>
  </tr>
  <tr>
    <td>Nome</td>
    <td>Um identificador exclusivo da notificação. Esse campo é obrigatório.</td>
  </tr>
  <tr>
    <td>Tipo</td>
    <td>Selecione: **Webhook**</td>
  </tr>
  <tr>
    <td>URL de webhook</td>
    <td>Insira a URL na qual o POST deve ser feito.</td>
  </tr>
  <tr>
  <td>Verificar certificados</td>
    <td>Selecione para verificar certificados.</td>
  </tr>
  <tr>
    <td>Cabeçalhos de webhook</td>
    <td>Insira quaisquer cabeçalhos.</td>
  </tr>
  <tr>
    <td>Parâmetros de consulta do webhook</td>
    <td>Insira quaisquer parâmetros de consulta.</td>
  </tr>
</table>

<table>
  <caption>Detalhes de notificação de obrigação do pager</caption>
  <tr>
     <th>Campo</th>
     <th>Descrição</th>
  </tr>
  <tr>
    <td>Nome</td>
    <td>Um identificador exclusivo da notificação. Esse campo é obrigatório.</td>
  </tr>
  <tr>
    <td>Tipo</td>
    <td>Selecione: **Obrigação do pager**</td>
  </tr>
  <tr>
    <td>Chave API</td>
    <td>Insira a chave API para notificações de obrigação do pager.</td>
  </tr>
</table>


5. Clique em **OK** para criar as novas notificações com a configuração especificada.

## Editar uma notificação
 1. Depois de instalar a versão beta, selecione **Dispositivos -> Monitoramento**. 
 2. Clique na guia **Notificações**.
3. Clique em **Ações -> Editar notificação**.
4. Edite qualquer um dos detalhes de notificação.
5. Clique em **OK** para aceitar suas mudanças.

## Excluir uma notificação
1. Depois de instalar a versão beta, selecione **Dispositivos -> Monitoramento**. 
2. Clique na guia **Notificações**.
3. Clique em **Ações -> Excluir notificação**.
4. Clique em **Excluir** para confirmar sua opção.

## Incluir múltiplas notificações em um dispositivo
1. Selecione **Infraestrutura->Lista de dispositivo->*Nome do dispositivo*** para acessar os detalhes do dispositivo.
2. Clique em **Ações -> Gerenciar notificações**.
4. Clique para designar ou remover notificações de seu dispositivo.

