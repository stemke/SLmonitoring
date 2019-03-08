---

copyright:
  years: 2018
lastupdated: "2018-04-20"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalando o IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)

Para permitir que o monitoramento avançado funcione no {{site.data.keyword.baremetal_short}} existente, siga estas etapas para instalar o {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent em seu dispositivo bare metal.

## Pré-requisitos
Deve-se estar conectado ao dispositivo bare metal para fazer download e executar os instaladores.

## Instalando no Windows

1. Faça download do instalador do IBM Cloud Monitoring Agent do Windows. [Download
![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi){: new_window}
2. Execute o instalador na máquina de destino.

## Instalando no Linux

1. Faça download do instalador do IBM Cloud Monitoring Agent do Linux. [Download ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz){: new_window}
2. Extraia-o na máquina de destino.
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. Execute o script linux_install.sh.


## Instalando no FreeBSD
1. Faça download do instalador do IBM Cloud Monitoring Agent do FreeBSD. [Download
![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz){: new_window}
2. Extraia-o na máquina de destino.
       `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. Execute o script freebsd_install.sh.

## Próximos passos

Depois de executar a instalação, o sistema concluirá o processo automaticamente. No Windows, aparecerá uma mensagem com uma confirmação de instalação bem-sucedida ou com informações sobre quaisquer erros que tiverem ocorrido.

Se você está usando um firewall, pode ser necessário permitir que o IBM Cloud Monitoring Agent transmita dados por meio dele. O agente usa a porta 8090 para comunicação HTTPS de saída. Para obter mais informações sobre endereços IP que você possa precisar permitir, veja [Intervalos de IP do balanceador de carga](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-load-balancer-ips#load-balancer-ips).
