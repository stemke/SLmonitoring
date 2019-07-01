---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords: IBM Cloud Monitoring, Standard Monitoring Services, Nimsoft Monitoring

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Guía de aprendizaje de iniciación
{: #monitoring}

{{site.data.keyword.cloud}} ofrece tanto servicios de supervisión estándar como servicios de supervisión Nimsoft para garantizar que el usuario siempre está al corriente de los problemas de sus dispositivos. Los servicios de supervisión estándar incluyen características como Ping y estadísticas de IPMI. Nimsoft Monitoring consta de tres niveles de supervisión, que incluyen la supervisión básica, avanzada y premium. Cada servicio de las ofertas de supervisión estándar y de Nimsoft ofrece varias ventajas y está disponible en varias opciones de precios para satisfacer sus necesidades empresariales. Para obtener más información, consulte [Supervisión e informes de la infraestructura de {{site.data.keyword.cloud}} ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://www.ibm.com/cloud/infrastructure/monitoring){:new_window}.
{:shortdesc}

La supervisión de un dispositivo le permite iniciar operaciones ping de servicio y lentas para asegurarse de que el dispositivo está en línea y responde.

Si no se recibe un eco durante el periodo de tiempo asignado (1 segundos para operaciones ping de servicio, 5 segundos para operaciones ping lentas), se envía una alerta a la dirección de correo electrónico especificada en la cuenta. El valor **Up (activo)** en el campo **Estado** indica que se ha recibido un eco y **Down (inactivo)** indica que no se ha recibido.

Para ver los supervisores configurados, siga estos pasos:

1. Navegue hasta el menú del dispositivo de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
2. En el menú **Dispositivos**, seleccione **Lista de dispositivos** y seleccione el dispositivo.
3. Pulse el separador **Supervisión**. Aparece una página en la que se ven todos los pings actuales. 

El separador **Supervisión** solo se puede ver si hay al menos un supervisor configurado.
{:note}

