---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalación y gestión de Nimsoft Monitoring Robot
{: #installing-and-managing-the-nimsoft-monitoring-robot}

Para que la supervisión avanzada funciones en {{site.data.keyword.baremetal_short}} o {{site.data.keyword.BluVirtServers_short}} existente, instale Nimsoft Monitoring Robot. Nimsoft Monitoring Robot permite que el sistema de gestión de supervisión se comunique con el servidor nativo o con el servidor virtual de la red privada. Después de instalar Nimsoft Monitoring Robot, tarda aproximadamente entre 5 y 10 minutos en estar disponible en la consola de {{site.data.keyword.cloud}}. Siga los siguientes pasos para instalar Nimsoft Monitoring Robot en Windows o Linux.

## Requisitos previos

Antes de instalarlo, estos puertos deben estar abiertos en la red privada:

* tcp/48000
* tcp/48001
* tcp/48002

Abra también los puertos de tcp/48003 a tcp/50000 para la red privada para permitir la funcionalidad completa que utiliza la API. Si no abre estos puertos, algunos agentes de supervisión se verán afectados. Si se encuentran errores durante la configuración, asegúrese de que estos puertos estén abiertos antes de abrir una incidencia para que se escale.

* Se necesita **openjdk** para ciertos agentes de supervisión, como por ejemplo Tomcat Monitoring Agent.
* Algunas distribuciones Linux de 64 bits necesitan **glibc.i686** y **nss-softtokn-freebl.i686**.
* El sistema de supervisión no recibe soporte en **FreeBSD**.

Si se produce un error al configurar el servicio de supervisión debido a errores de comunicación con el robot Nimsoft, el proceso de configuración se puede poner en pausa debido a la conectividad limitada. La conectividad limitada suele deberse a un cortafuegos o a otro software de seguridad que bloquea el acceso al sistema desde los servidores de gestión Nimsoft. Siga estos pasos para reiniciar el suministro del servicio de supervisión:

## Reinicio del suministro de un agente de supervisión
{: #restarting-provisioning-of-a-monitoring-agent}

Siga los siguientes pasos para reiniciar el suministro del servicio de supervisión.
1. Navegue hasta el menú del dispositivo de la consola. Para obtener más información, consulte [Navegación a dispositivos](https://test.cloud.ibm.com/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
2. En el menú **Dispositivos**, seleccione **Supervisión**.
3. Busque el sistema para el que se está configurando la supervisión.
4. Seleccione **"Volver a desplegar todos los agentes"** en la sección **Avanzado**.
5. Seleccione una plantilla de supervisión en la página **Pop-In**.
6. Pulse **Volver a desplegar**.

## Instalación en Windows
{: #install-windows}

1. Consulte http://downloads.service.softlayer.com/nimsoft/ para descargar la última versión del instalador de Windows en el dispositivo para instalarlo (debe estar conectado al cliente VPN).
2. Ejecute el archivo Nimsoft Monitoring Robot como administrador.

## Instalación en Linux
{: #install-linux}

1. Conéctese a la red privada a través del cliente VPN.
2. Descargue el instalador de Linux de [32 bits ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} o de [64 bits ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} en el dispositivo para la instalación. Las versiones de Debian y Ubuntu también están disponibles en el [instalador de Nimsoft ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://downloads.service.softlayer.com/nimsoft/){: new_window}.
3. Ejecute estos mandatos para completar la instalación y sustituya 32 por 64 si ejecuta una instalación de 64 bits:

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Siguientes pasos

Después de ejecutar la instalación, el sistema completa el proceso automáticamente. En Windows, aparece un mensaje con una confirmación de una instalación correcta o con información sobre los errores que se han producido.

