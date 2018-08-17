---
copyright:
  years: 2018
lastupdated: "2018-04-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalación de IBM Cloud Monitoring Service para el agente nativo IaaS (Beta)

Para que la supervisión avanzada funcione en los {{site.data.keyword.baremetal_short}} existentes, siga estos pasos para instalar {{site.data.keyword.BluSoftlayer_full}} Monitoring Service para el agente nativo IaaS en el dispositivo nativo.

## Requisitos previos
Debe estar conectado al dispositivo nativo para descargar y ejecutar los instaladores.

## Instalación en Windows

1. Descargue el instalador de Windows IBM Cloud Monitoring Agent. [Descarga](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi)
2. Ejecute el instalador en la máquina de destino. 

## Instalación en Linux

1. Descargue el instalador de Linux IBM Cloud Monitoring Agent. [Descarga](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz)
2. Descomprímalo en la máquina de destino. 
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. Ejecute el script linux_install.sh.

        
## Instalación en FreeBSD
1. Descargue el instalador de FreeBSD IBM Cloud Monitoring Agent. [Descarga](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz)
2. Descomprímalo en la máquina de destino. 
       `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. Ejecute el script freebsd_install.sh. 

## Siguientes pasos

Después de ejecutar la instalación, el sistema completa el proceso automáticamente. En Windows, aparece un mensaje con una confirmación de una instalación correcta o con información sobre los errores que se han producido.

Si utiliza un cortafuegos, es posible que tenga que permitir que IBM Cloud Monitoring Agent pase datos a través del mismo.  El agente utiliza el puerto 8090 para la comunicación HTTPS de salida. Para obtener más información sobre las direcciones IP que es posible que tenga que permitir, consulte el apartado sobre [Rangos de IP del equilibrador de carga](https://console.bluemix.net/docs/infrastructure/hardware-firewall-dedicated/ips.html#load-balancer-ips).
