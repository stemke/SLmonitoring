---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Exploraciones de vulnerabilidades
{{site.data.keyword.BluSoftlayer_full}} se asocia con Nessus para ofrecer exploraciones de vulnerabilidades para cualquier dispositivo de la red de {{site.data.keyword.BluSoftlayer_notm}}.  Las exploraciones de vulnerabilidades realizan pruebas para detectar los puntos débiles de un dispositivo y devuelven un informe del análisis, los problemas de seguridad y los arreglos disponibles para el dispositivo de host.  La realización de exploraciones de vulnerabilidades en sus dispositivos garantizan su seguridad en todo momento y también constituyen el primer recurso que utilizar cuando se cree que un dispositivo puede resultar vulnerable.  Las exploraciones de vulnerabilidades se pueden completar mediante el [Portal de clientes ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/) en cualquier dispositivo asociado con su cuenta.
{:shortdesc}

## Explorador de seguridad de Nessus 
{{site.data.keyword.BluSoftlayer_notm}} proporciona un explorador de seguridad en línea, basado en la herramienta de código abierto Nessus Scanning. Se puede acceder a este explorador de seguridad desde el separador Seguridad pulsando en **Explorador**. Para obtener más información, consulte el tema sobre la [herramienta Nessus Scanning ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://www.nessus.org/nessus/).

La página **Explorador** proporciona una lista del hardware disponible para la herramienta Nessus alojada en {{site.data.keyword.BluSoftlayer_notm}}. Para explorar un servidor, o para ver los resultados de una exploración anterior, pulse el enlace de detalles correspondiente al servidor que desea inspeccionar. La página de detalles de la exploración de vulnerabilidades muestra un breve resumen del servidor (que contiene el nombre del servidor, la dirección IP que se debe explorar y el centro de datos donde se encuentra el servidor). **Iniciar exploración** planifica su servidor con el servidor de exploración de Nessus para realizar una exploración de vulnerabilidades lo antes posible.

Después del resumen del servidor hay una tabla de las exploraciones de vulnerabilidades de Nessus anteriores y actuales. Para cada exploración se muestra la fecha en que se ha solicitado la exploración, la fecha en que se ha iniciado la exploración, el estado de la exploración y, si la exploración ha finalizado, un enlace con el informe de Nessus.

Los informes de Nessus pueden tener uno de estos estados:

* Pendiente de exploración: la exploración se ha planificado para el recuadro del explorador de Nessus.
* Exploración en proceso: la exploración se está procesando actualmente.
* Generando informe: la exploración ha finalizado y los resultados se están compilando en un informe.
* Exploración finalizada: la exploración ha finalizado correctamente y se ha generado el informe de vulnerabilidades.
* Exploración cancelada: un técnico de {{site.data.keyword.BluSoftlayer_notm}} ha cancelado manualmente la exploración de Nessus.

Si se pulsa **Ver informe** se puede ver un informe correspondiente a cada exploración de Nessus finalizada correctamente. El informe contiene dos tablas: una tabla de detalles de la exploración, que muestra el número de hosts que se han explorado, el número de vulnerabilidades de seguridad abiertas (agujeros) que se han encontrado y el número de posibles vulnerabilidades de seguridad (avisos) que se han encontrado. La segunda tabla muestra todos los problemas de seguridad encontrados: el host en el que se ha encontrado la vulnerabilidad y una descripción de la posible vulnerabilidad.

La herramienta Nessus de código abierto es un plugin, lo que permite desarrollar nuevas pruebas a medida que se encuentran vulnerabilidades. {{site.data.keyword.BluSoftlayer_notm}} actualiza la herramienta interna de Nessus con regularidad, por lo que se recomienda realizar una exploración regular con el explorador de seguridad para mantenerse al día con las nuevas amenazas.

Para que la exploración se realice correctamente, las conexiones desde 173.192.255.232 y 172.17.19.38 deben tener permiso para acceder al servidor.
