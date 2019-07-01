---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

# Perguntas Frequentes
{: #monitoring-faq}

## Estou vendo vários chamados de alerta de monitoramento. Isso significa que meu servidor está inativo?
{: faq}

Cada dispositivo vem com um ping de monitoramento e um serviço de notificação complementar. Este serviço cria automaticamente um chamado de alerta de monitoramento em caso de falha de parâmetros configurados. Falsos positivos são possíveis com o serviço de monitoramento e podem ser atribuídos à limitação de taxa por um firewall de software na disponibilidade do servidor, do serviço e do aplicativo, além de interrupções de serviço na infraestrutura de monitoramento. Revise as configurações padrão para minimizar possíveis falsos alertas de monitoramento.

## Posso deixar que o sistema de monitoramento emita uma reinicialização automática e alerte um técnico de suporte se o servidor parar de responder?
{: faq}

Sim, com o serviço **Automated Reboot from Monitoring Failure**, será possível configurar o sistema de monitoramento para reinicializar automaticamente o servidor e emitir um chamado para um técnico de suporte se um alerta de monitoramento for emitido.

## Qual é a diferença entre o monitoramento com um "ping lento" e um "ping de serviço"?
{: faq}

A diferença entre um ping de serviço e um ping lento é o período de tempo em que uma resposta de um dispositivo é esperada. O padrão é o ping de serviço, mas é possível mudar para usar um ping lento, como alternativa.

* Um ping de **serviço** emite um ping a cada 5 minutos e espera uma resposta de eco em 1 segundo. Se mais de um ping for perdido, um alerta será emitido.
* Um ping **lento** aguarda 5 segundos por uma resposta, permitindo aos servidores otimizados para tarefas que não são da rede mais tempo para processar a solicitação.


## Quando um chamado de monitoramento for aberto e me alertar sobre o problema, os técnicos verão o chamado e responderão?
{: faq}

Com o serviço de ping básico, os técnicos de suporte não são notificados de falhas. Esses chamados são abertos quando o sistema de monitoramento emite um alerta e eles notificam apenas os usuários especificados na tela de monitoramento. Os
técnicos não são alertados até que você abra um novo chamado indicando que o servidor não está respondendo.


## Quando um chamado de monitoramento for aberto e me alertar sobre o problema, os técnicos verão o chamado e responderão?
{: faq}

Com o serviço de ping básico, os técnicos de suporte não são notificados de falhas. Esses chamados são abertos quando o sistema de monitoramento emite um alerta e eles notificam apenas os usuários especificados na tela de monitoramento. Os
técnicos não são alertados até que você abra um novo chamado indicando que o servidor não está respondendo.
