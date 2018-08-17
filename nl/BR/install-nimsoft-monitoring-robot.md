---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalando e gerenciando o Nimsoft Monitoring Robot

Para permitir que o monitoramento avançado funcione no {{site.data.keyword.baremetal_short}} ou {{site.data.keyword.BluVirtServers_short}} existentes, instale o Nimsoft Monitoring Robot. O Nimsoft Monitoring Robot permite que o sistema de gerenciamento de monitoramento se comunique com o servidor bare metal ou servidor virtual na rede privada. Após a instalação do Nimsoft Monitoring Robot, ele leva aproximadamente de 5 a 10 minutos para se tornar disponível no {{site.data.keyword.slportal_full}}. Siga estas etapas para instalar o Nimsoft Monitoring Robot no Windows ou Linux.

## Pré-requisitos

Antes de instalar, estas portas devem ser abertas na rede privada:

* tcp/48000
* tcp/48001
* tcp/48002

Além disso, abra as portas tcp/48003 a tcp/50000 da rede privada para permitir a funcionalidade completa usada pela API. Se você não abrir essas portas, alguns agentes de monitoramento serão afetados. Se forem encontrados erros durante a configuração, assegure-se de que essas portas estejam abertas antes de abrir um chamado para escalação. 

* **openjdk** necessário para alguns agentes de monitoramento, como o Tomcat Monitoring Agent.
* Algumas distribuições Linux de 64 bits requerem **glibc.i686** e **nss-softtokn-freebl.i686**.
* O sistema de monitoramento não é suportado no **FreeBSD**.
* O sistema de monitoramento não é suportado no **Ubuntu 16**.
* O sistema de monitoramento não é suportado no **Windows 2016**.

Se houver um erro ao configurar o serviço de monitoramento devido a erros de comunicação com o robô Nimsoft, o processo de configuração poderá ser pausado devido à conectividade limitada. A conectividade limitada é muitas vezes causada pelo firewall ou outro software de segurança que está bloqueando o acesso ao sistema por meio dos servidores de gerenciamento Nimsoft. Siga estas etapas para reiniciar o fornecimento do serviço de monitoramento:

## Reiniciando o fornecimento de um agente de monitoramento

1. Acesse o menu **Dispositivos** e selecione **Monitoramento**.
* Localize o sistema para o qual o monitoramento está sendo configurado.
* Selecione **"Reimplementar todos os agentes"** na lista suspensa **Avançado** na coluna da direita.
* Escolha um modelo de monitoramento na página **Entrada de pop**.
* Clique em **Reimplementar**

## Instalando no Windows

1. Veja http://downloads.service.softlayer.com/nimsoft para fazer download da versão mais recente do Windows Installer no dispositivo para instalação (Deve-se estar conectado à VPN).
* Execute o arquivo Nimsoft Monitoring Robot como um Administrador.

## Instalando no Linux

1. Conecte-se à rede privada por meio da VPN.
* Faça download do Linux Installer de [32 bits](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz) ou [64 bits](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz) no dispositivo para instalação. As versões Debian e Ubuntu também estão disponíveis no [Nimsoft Installer](http://downloads.service.softlayer.com/nimsoft/).
* Execute estes comandos para concluir a instalação, substituindo 32 por 64, se você estiver executando uma instalação de 64 bits:

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Próximos passos

Depois de executar a instalação, o sistema concluirá o processo automaticamente. No Windows, aparecerá uma mensagem com uma confirmação de instalação bem-sucedida ou com informações sobre quaisquer erros que tiverem ocorrido.
