---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Métricas coletadas (Beta)
Este tópico abrange as métricas coletadas para este aplicativo de monitoramento beta em servidores virtuais e bare metal.
{:shortdesc}

Este tópico abrange todas as métricas disponíveis por meio de consultas no Grafana. Para obter mais informações, veja [Criando uma consulta de monitoramento avançada (Beta)](advanced_query.html). Há gráficos disponíveis na interface com o usuário somente para as métricas a seguir:
* Utilização da CPU
* Uso de memória
* Leitura e gravação do disco (bytes/segundos e E/S por segundo)
* Latência de leitura e gravação do disco
* Rendimento da rede pública (entrada/saída)
* Rendimento da rede privada (entrada/saída)
* Pacotes da rede pública (entrada/saída) (Bare metal somente)
* Pacotes da rede privada (entrada/saída) (Bare metal somente)
* Erros da rede pública (entrada/saída) (Bare metal somente)
* Erros da rede privada (entrada/saída) (Bare metal somente)
* Temperatura (Bare metal somente)


## Métricas de CPU
  As métricas de CPU medem a porcentagem média de tempo que uma CPU está executando instruções durante um determinado período. A porcentagem média inativa fica inativa com a adição de usuário, nice, sistema, espera de E/S, interrupções de hardware e interrupções de software.

## Métricas de memória
* Bytes usados/Média usada: a quantia de memória que está sendo usada em um determinado momento, disponível tanto em bytes quanto na porcentagem do total.
* Bytes de troca usados/Média usada: a porcentagem de memória de troca que está sendo usada durante um determinado período. Essa métrica é uma indicação de quantas vezes você tem que recuperar dados que não estão na memória. Essa métrica está disponível somente em dispositivos bare metal.
  
## Métricas de disco

* Total do disco: a quantia total de bytes disponíveis para o disco. Essa métrica deve ser constante.
* Disco usado (Bytes): a quantia de bytes que estão sendo usados pelo disco no momento especificado.
* Disco usado (Porcentagem): a porcentagem da quantia total de bytes que estão sendo usados sobre a quantia total de bytes disponíveis para o disco.
* Leitura/gravação de disco (bytes por segundo): a quantia média de dados que estão sendo lidos/gravados do disco/no disco, em bytes, por um determinado período.
* Leitura/gravação de disco (operações por segundo): operações de leitura/gravação por segundo
* Leitura/gravação de disco (latência em ms por operação): latência em ms por leitura/gravação

## Métricas de rede

 * Entrada de rede Pública/Privada: número de bytes enviados pela rede Pública/Privada
* Saída de rede Pública/Privada: número de bytes recebidos pela rede Pública/Privada
* Entrada de pacotes de rede Pública/Privada: número de pacotes recebidos pela interface de rede na rede Pública/Privada. Essa métrica está disponível somente em dispositivos bare metal.
* Saída de pacotes de rede Pública/Privada: número de pacotes enviados pela interface de rede na rede Pública/Privada. Essa métrica está disponível somente em dispositivos bare metal.

## Métricas de temperatura
* A temperatura média do sistema medida em graus Celsius. Essa métrica está disponível apenas em dispositivos bare metal selecionados.



