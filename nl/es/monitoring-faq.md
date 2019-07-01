---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

# Preguntas frecuentes
{: #monitoring-faq}

## Veo varias incidencias de alertas de supervisión. ¿Significa esto que mi servidor está inactivo?
{: faq}

Cada dispositivo viene con un servicio complementario de notificación y ping de supervisión. Este servicio crea automáticamente una incidencia de alerta de supervisión según los parámetros establecidos con errores. Es posible que se produzcan falsos positivos con el servicio de supervisión que se pueden atribuir a una limitación de velocidad impuesta por un cortafuegos en el servidor, a la disponibilidad del servicio y de la aplicación y a interrupciones del servicio en la infraestructura de supervisión. Revise los valores predeterminados para mitigar las posibles alertas de supervisión falsas.

## ¿Puedo hacer que el sistema de supervisión emita un rearranque automático y avise a un técnico de soporte si el servidor deja de responder?
{: faq}

Sí, con el servicio **Rearranque automático después de un error de supervisión** puede configurar el sistema de supervisión de modo que rearranque automáticamente el servidor y emita una incidencia destinado a un técnico de soporte si se emite una alerta de supervisión.

## ¿Qué diferencia hay entre la supervisión con un "ping lento" y un "ping de servicio"?
{: faq}

La diferencia entre un ping de servicio y un ping lento es el intervalo de tiempo en el que se espera recibir una respuesta del dispositivo. El valor predeterminado es el ping de servicio, pero puede modificarlo para utilizar en su lugar un ping lento.

* Un ping de **servicio** emite un ping cada 5 minutos y espera una respuesta de eco en un plazo de 1 segundo. Si se ha perdido más de un ping, se emite una alerta.
* Un ping **lento** espera una respuesta durante 5 segundos, lo que permite que los servidores que están optimizados para tareas que no son de red tengan más tiempo para procesar la solicitud.


## Cuando se abre una incidencia de supervisión y me alerta sobre el problema, ¿verán los técnicos la incidencia y responderán?
{: faq}

Con el servicio de ping básico, no se notifica a los técnicos de soporte sobre los errores. Estas incidencias se abren cuando el sistema de supervisión emite una alerta, y solo notifican a los usuarios que especifique en la pantalla de supervisión. No se alerta a los técnicos hasta que el usuario abre una nueva incidencia que indique que el servidor no responde.


## Cuando se abre una incidencia de supervisión y me alerta sobre el problema, ¿verán los técnicos la incidencia y responderán?
{: faq}

Con el servicio de ping básico, no se notifica a los técnicos de soporte sobre los errores. Estas incidencias se abren cuando el sistema de supervisión emite una alerta, y solo notifican a los usuarios que especifique en la pantalla de supervisión. No se alerta a los técnicos hasta que el usuario abre una nueva incidencia que indique que el servidor no responde.
