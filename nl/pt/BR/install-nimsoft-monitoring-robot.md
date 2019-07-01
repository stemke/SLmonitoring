---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalando e gerenciando o Nimsoft Monitoring Robot
{: #installing-and-managing-the-nimsoft-monitoring-robot}

Para permitir que o monitoramento avançado funcione no {{site.data.keyword.baremetal_short}} ou {{site.data.keyword.BluVirtServers_short}} existentes, instale o Nimsoft Monitoring Robot. O Nimsoft Monitoring Robot permite que o sistema de gerenciamento de monitoramento se comunique com o servidor bare metal ou servidor virtual na rede privada. Depois de instalar o Nimsoft Monitoring Robot, leva aproximadamente 5
a 10 minutos para ficar disponível no console do {{site.data.keyword.cloud}}. Conclua as etapas a seguir para instalar o Nimsoft Monitoring Robot no Windows ou Linux.

## Pré-requisitos

Antes de instalar, estas portas devem ser abertas na rede privada:

* tcp/48000
* tcp/48001
* tcp/48002

Além disso, abra as portas tcp/48003 a tcp/50000 da rede privada para permitir a funcionalidade completa usada pela API. Se você não abrir essas portas, alguns agentes de monitoramento serão afetados. Se forem encontrados erros durante a configuração, assegure-se de que essas portas estejam abertas antes de abrir um chamado para escalação.

* **openjdk** necessário para alguns agentes de monitoramento, como o Tomcat Monitoring Agent.
* Algumas distribuições Linux de 64 bits requerem **glibc.i686** e **nss-softtokn-freebl.i686**.
* O sistema de monitoramento não é suportado no **FreeBSD**.

Se houver um erro ao configurar o serviço de monitoramento devido a erros de comunicação com o robô Nimsoft, o processo de configuração poderá ser pausado devido à conectividade limitada. A conectividade limitada é muitas vezes causada pelo firewall ou outro software de segurança que está bloqueando o acesso ao sistema por meio dos servidores de gerenciamento Nimsoft. Siga estas etapas para reiniciar o fornecimento do serviço de monitoramento:

## Reiniciando o fornecimento de um agente de monitoramento
{: #restarting-provisioning-of-a-monitoring-agent}

Conclua as etapas a seguir para reiniciar o fornecimento do serviço de monitoramento.
1. Navegue para o menu de dispositivos do console. Para obter mais informações, consulte [Navegando para os dispositivos](https://test.cloud.ibm.com/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
2. No menu **Dispositivos**, selecione **Monitoramento**.
3. Localize o sistema para o qual o monitoramento está sendo configurado.
4. Selecione **"Reimplementar todos os agentes"** na seção **Avançado**.
5. Escolha um modelo de monitoramento na página **Entrada de pop**.
6. Clique em **Reimplementar**.

## Instalando no Windows
{: #install-windows}

1. Consulte http://downloads.service.softlayer.com/nimsoft/ para fazer download da versão mais recente do Windows Installer para o dispositivo a ser instalado (deve-se estar conectado à VPN do cliente).
2. Execute o arquivo Nimsoft Monitoring Robot como um Administrador.

## Instalando no Linux
{: #install-linux}

1. Conecte-se à rede privada por meio da VPN do cliente.
2. Faça download do [de 32 bits ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} ou do [ ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} Linux Installer de 64 bits para o dispositivo a ser instalado. As versões Debian e Ubuntu também estão disponíveis no [Nimsoft Installer ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://downloads.service.softlayer.com/nimsoft/){: new_window}.
3. Execute estes comandos para concluir a instalação, substituindo 32 por 64, se você estiver executando uma instalação de 64 bits:

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Próximos passos

Depois de executar a instalação, o sistema concluirá o processo automaticamente. No Windows, aparecerá uma mensagem com uma confirmação de instalação bem-sucedida ou com informações sobre quaisquer erros que tiverem ocorrido.

