---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalación y gestión de Nimsoft Monitoring Robot

Para que la supervisión avanzada funciones en {{site.data.keyword.baremetal_short}} o {{site.data.keyword.BluVirtServers_short}} existente, instale Nimsoft Monitoring Robot. Nimsoft Monitoring Robot permite que el sistema de gestión de supervisión se comunique con el servidor nativo o con el servidor virtual de la red privada. Después de instalar Nimsoft Monitoring Robot, tarda aproximadamente entre 5 y 10 minutos en estar disponible en el {{site.data.keyword.slportal_full}}. Siga estos pasos para instalar Nimsoft Monitoring Robot en Windows o Linux.

## Requisitos previos

Antes de instalarlo, estos puertos deben estar abiertos en la red privada:

* tcp/48000
* tcp/48001
* tcp/48002

Abra también los puertos de tcp/48003 a tcp/50000 para la red privada para permitir la funcionalidad completa que utiliza la API. Si no abre estos puertos, algunos agentes de supervisión se verán afectados. Si se encuentran errores durante la configuración, asegúrese de que estos puertos estén abiertos antes de abrir una incidencia para que se escale. 

* Se necesita **openjdk** para ciertos agentes de supervisión, como por ejemplo Tomcat Monitoring Agent.
* Algunas distribuciones Linux de 64 bits necesitan **glibc.i686** y **nss-softtokn-freebl.i686**.
* El sistema de supervisión no recibe soporte en **FreeBSD**.
* El sistema de supervisión no recibe soporte en **Ubuntu 16**.
* El sistema de supervisión no recibe soporte en **Windows 2016**.

Si se produce un error al configurar el servicio de supervisión debido a errores de comunicación con el robot Nimsoft, el proceso de configuración se puede poner en pausa debido a la conectividad limitada. La conectividad limitada suele deberse a un cortafuegos o a otro software de seguridad que bloquea el acceso al sistema desde los servidores de gestión Nimsoft.  Siga estos pasos para reiniciar el suministro del servicio de supervisión:

## Reinicio del suministro de un agente de supervisión

1. Vaya al menú **Dispositivos** y seleccione **Supervisión**.
* Busque el sistema para el que se ha configurado la supervisión.
* Seleccione **"Volver a desplegar todos los agentes"** en el menú desplegable **Avanzado** en la columna de la derecha.
* Seleccione una plantilla de supervisión en la página **Pop-In**.
* Pulse **Volver a desplegar**

## Instalación en Windows

1. Consulte http://downloads.service.softlayer.com/nimsoft para descargar la última versión del instalador de Windows en el dispositivo para instalarlo (debe estar conectado a VPN).
* Ejecute el archivo Nimsoft Monitoring Robot como administrador.

## Instalación en Linux

1. Conéctese a la red privada a través de VPN.
* Descargue el instalador de Linux de [32 bits](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz) o de [64 bits](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz) en el dispositivo para instalarlo. Las versiones de Debian y Ubuntu también están disponibles en el [instalador de Nimsoft](http://downloads.service.softlayer.com/nimsoft/).
* Ejecute estos mandatos para completar la instalación y sustituya 32 por 64 si ejecuta una instalación de 64 bits:

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## Siguientes pasos

Después de ejecutar la instalación, el sistema completa el proceso automáticamente. En Windows, aparece un mensaje con una confirmación de una instalación correcta o con información sobre los errores que se han producido.
