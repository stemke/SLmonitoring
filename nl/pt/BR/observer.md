Um administrador pode obter uma visualização holística do funcionamento atual e passado de seu dispositivo em um local.

Histórias do usuário:

    Qualquer usuário pode alternar rapidamente as guias "Largura de banda" e "Uso" entre sua visualização existente e o beta Observer (BETA somente)

    Qualquer usuário pode fornecer feedback sobre sua experiência no beta Observer por meio do portal de Controle (BETA somente)

    Qualquer usuário pode acessar o blog posteriormente para saber mais sobre nosso trabalho no Observer dentro da experiência beta (BETA somente)

    Os usuários têm um local designado no qual podem armazenar e visualizar métricas do recurso de infraestrutura para servidores virtuais:

    1. Utilização da CPU, %, por núcleo virtual

    2. Rede - pública, entrada/saída, bytes e pacotes

    3. Rede - privada, entrada/saída, bytes e pacotes

    4. Utilização de memória, %

    5. Leitura do disco, bytes e operações

    6. Gravação no disco, bytes e operações

    7. Erros de transmissão, entrada/saída, contagem

    8. Latência do disco, ms, leitura e gravação

    9. Utilização do disco local, % e bytes usados e total de bytes disponíveis


    Os usuários do bare metal poderão visualizar as métricas a seguir:

    1. Utilização da CPU, %, por núcleo virtual

    2. Rede - pública, entrada/saída, bytes e pacotes

    3. Rede - privada, entrada/saída, bytes e pacotes

    4. Utilização de memória, %

    5. Leitura do disco, bytes e operações

    6. Gravação no disco, bytes e operações

    7. Erros de transmissão, entrada/saída, contagem

    8. Latência do disco, ms, leitura e gravação

    9. Utilização do disco local, % e bytes usados e total de bytes disponíveis

    10. Alertas do RAID, 0/1

    11. Temperatura do núcleo, graus F

    Qualquer administrador pode visualizar o histórico de alarmes e métricas em uma única visualização sem precisar fazer qualquer análise de criação de log. (semelhante a #60)

    Um gerenciador pode entender o funcionamento geral de seu dispositivo sem precisar de esclarecimento de suas equipes de administração.

    Qualquer usuário pode abrir o arquivo syslog mais recente de um dispositivo sem usar a linha de comandos (semelhante a #35)

    Qualquer usuário pode visualizar e explorar quaisquer dados de métrica de série temporal em um conjunto de gráficos interativos.

    Qualquer usuário pode visualizar e ter uma noção básica do histórico de alerta.

    Qualquer usuário pode marcar os eventos como "aberto" ou "fechado".

    Nenhum usuário precisa criar manualmente um evento sempre que um alarme é acionado.

    Nenhum usuário precisa designar manualmente um nível de severidade de "aviso" ou "erro" além de suas configurações de alarme.

    Qualquer usuário pode reunir métricas no nível do sistema e do aplicativo usando agentes collectD para monitorar respostas de processos, apache, tomcat, MSSQL, MySQL e URL.

    Um administrador pode enviar dados de métrica customizados para o serviço de monitoramento de uma maneira automatizada.

    Qualquer usuário pode utilizar métricas do sistema, do aplicativo ou customizadas da mesma maneira que métricas do hypervisor: gráficos, painéis, alarmes, notificações, respostas automáticas, modelos, etc.



Hill 2: um administrador pode entender e começar a solucionar problemas de um incidente em 90 segundos

Histórias do usuário:

    Qualquer administrador pode assinar alertas sem ser inundado com falsos positivos.

    Qualquer administrador pode receber alertas por meio de sua primeira escolha de canal de comunicação em um minuto de um evento acionador.

    Os engenheiros de confiabilidade podem entender a causa de um alerta de incidente com base na mensagem no próprio alerta.

    Qualquer administrador pode verificar métricas de uso recentes em qualquer dispositivo com um alto grau de precisão.

    Qualquer administrador pode procurar as informações exatas que precisa em menos de 10 segundos.

    Um não administrador pode resolver um incidente escalado com menos de três mensagens do suporte SL

    Qualquer usuário pode especificar uma condição para o alerta de qualquer métrica disponível (padrão, collectD ou customizado).

    Qualquer usuário pode especificar uma condição com base no valor médio, valor acumulativo (soma), valor mínimo ou valor máximo de qualquer métrica.

    Qualquer usuário pode especificar uma condição com a qualificação "maior que" ou "menor que".

    Qualquer usuário pode especificar o número de períodos consecutivos a que uma condição deve ser atendida, bem como o comprimento do período, 30 segundos ou 5 minutos, antes de um alarme ser acionado - "se X ocorrer por 2 períodos consecutivos de 30 segundos, o alarme será acionado"

    Qualquer usuário pode especificar múltiplas condições para um único alarme - "se isto E isto E isto, então o alarme será acionado".

    Qualquer usuário pode especificar um nome customizado para o alarme.

    Qualquer usuário pode ser informado sobre alertas que indicam o tempo, o nome do alarme e as condições que foram atendidas que acionaram o alarme.

    Nenhum usuário, após um alarme ser acionado, receberá alertas adicionais da mesma regra no mesmo dispositivo até que o alarme inicial tenha sido "fechado".

    Exemplo de regra de alarme: se a média de Utilização de CPU for maior que 80% por 2 períodos consecutivos de 5 minutos E a soma da entrada de Rede for maior que 50 GB por 1 período consecutivo de 5 minutos, um alarme será acionado e um evento será criado (supondo que qualquer alarme anterior dessa regra tenha sido fechado)

    Um administrador pode especificar 1 ou mais endereços de e-mail para notificar qualquer usuário.

    Um administrador pode especificar 1 ou mais números de telefone SMS para notificar qualquer usuário.

    Um administrador pode especificar 1 ou mais URLs para envio pelos webhooks.

    Um administrador pode especificar o grupo Pagerduty para notificar os usuários.

    Um administrador pode especificar se o servidor deve ser reinicializado ou encerrado quando o alarme é acionado.

    Um administrador pode especificar um intervalo de 30 segundos ou 5 minutos para monitoramento de rede de qualquer protocolo suportado

    Um administrador pode implementar verificações de ping do host (ICMP)

    Um administrador pode implementar verificações de porta TCP para vários protocolos: DNS, DNS customizado, FTP, HTTP, HTTP customizado, HTTPS, IMAP, LDAP, NNTP, POP, SMTP, SSH, TCP customizado, TELNET, UDP SIP (existe suporte para esses protocolos na oferta SL TCP atual)

    Um administrador pode implementar uma verificação de porta TCP para o protocolo SNMP (não suportado atualmente na oferta SL existente)

    Um administrador pode especificar limite para o tempo de resposta se qualificar como um sucesso ou um erro

    Um administrador pode especificar o número de erros consecutivos de um ping do host ou de uma verificação de porta TCP antes de um alarme ser acionado.

    Um administrador pode implementar as mesmas opções de resposta de notificação e automatizada de alarmes de monitoramento de rede que de alarmes com base em métricas (e-mail, SMS, webhook, PagerDuty, reinicialização, encerramento)

    Um administrador pode especificar o nível de severidade de "aviso" ou "erro" para ambos os alarmes de monitoramento de métrica e de rede.



Hill 3: qualquer usuário pode configurar o monitoramento em qualquer dispositivo, gastando menos de 90 segundos em decisões de configuração. (semelhante a #59)

Histórias do usuário:

    Um não administrador pode configurar basicamente seu monitoramento usando apenas a interface e a documentação.

    Um administrador pode configurar o monitoramento que atende às suas necessidades específicas selecionando configurações salvas ou predefinidas sem passar pelo processo de configuração manual. (semelhante a #58)

    Um administrador pode configurar o monitoramento que atende às suas necessidades específicas editando e salvando manualmente uma configuração e aplicando-a a qualquer número de dispositivos.

    Um administrador pode configurar alertas em múltiplos dispositivos com o mínimo esforço repetitivo.

    Qualquer usuário pode exportar dados específicos de tempo e métrica em um arquivo CSV.

    Um administrador ou um gerenciador pode configurar uma janela de manutenção durante a qual nenhuma notificação será enviada quando alarmes forem acionados.

    Qualquer usuário estabelecido pode entender e aplicar as configurações salvas. (semelhante a #41)

    Qualquer novo usuário pode entender e aplicar configurações predefinidas. (semelhante a #34, #32)

    Um não administrador pode obter suporte ao configurar o monitoramento sem arquivar um chamado de suporte.

    Qualquer cliente pode solicitar monitoramento para qualquer dispositivo sem conhecimento de especialista. (semelhante a #63, #43)

    Todos os clientes têm uma experiência previsível unificada para pedir monitoramento para qualquer dispositivo. (semelhante a #40)

    Qualquer usuário pode integrar seu dispositivo a um serviço de terceiro sem arquivar um chamado de suporte.

    Nenhum usuário precisa criar manualmente um alarme para alertas de "aviso" de ciclo de vida: criação, inicialização, encerramento.

    Qualquer usuário técnico pode acessar toda a funcionalidade do Observer por meio da mesma API que o resto do serviço de monitoramento.

    A IBM pode restringir às contas ab o acesso a determinados recursos/desempenho com versão gratuita, conforme definido na Visão geral do Observer para a camada grátis vs. pago.

    Qualquer cliente pode fazer upgrade da versão gratuita para a versão paga dentro da guia de monitoramento.

    Qualquer cliente pode fazer upgrade ou downgrade de versões pagas ou gratuitas na área de gerenciamento de conta.

    Qualquer usuário com a versão gratuita pode visualizar as opções que teria se fizessem o upgrade, mas de uma forma que indica por que estão indisponíveis

    Se um usuário tentar executar uma ação que exija a execução de um upgrade, ele deverá ver uma mensagem explicando que precisa fazer upgrade e oferecendo uma alternativa, se uma existir (por exemplo, "Você já tem o número máximo de alarmes para a versão gratuita. Faça upgrade ou exclua um alarme para criar uma nova regra").


