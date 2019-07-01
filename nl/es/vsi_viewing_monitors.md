---

copyright:
  years: 2017, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:note: .note}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Visualización y gestión de supervisores
{: #viewing-and-managing-monitors}

La supervisión de un dispositivo le permite iniciar operaciones ping de servicio y lentas para asegurarse de que el dispositivo está en línea y responde.
{:shortdesc}

Si no se recibe un eco durante el periodo de tiempo asignado (1 segundos para operaciones ping de servicio, 5 segundos para operaciones ping lentas), se envía una alerta a la dirección de correo electrónico especificada en la cuenta. El valor **Up (activo)** en el campo **Estado** indica que se ha recibido un eco y **Down (inactivo)** indica que no se ha recibido. Si dispone de un supervisor básico configurado, siga estos pasos para ver y gestionar la supervisión de un dispositivo.

## Antes de empezar
Primero, navegue hasta el menú del dispositivo y asegúrese de tener los permisos de cuenta correctos para completar las tareas.

* Navegue hasta el menú del dispositivo de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Asegúrese de que tiene los permisos de cuenta y el acceso de dispositivo necesarios. Solo el propietario de la cuenta, o un usuario con el permiso de la infraestructura clásica **Gestionar usuarios**, puede ajustar los permisos.

Para obtener más información sobre permisos, consulte [Permisos de la infraestructura clásica](/docs/iam?topic=iam-infrapermission#infrapermission) y [Gestión del acceso a dispositivos](/docs/vsi?topic=virtual-servers-managing-device-access).

## Visualización de supervisores
{: #viewing-monitors}

1. En el menú **Dispositivos**, seleccione **Lista de dispositivos**.
2. Pulse el nombre de dispositivo para acceder al dispositivo.
3. Pulse el separador **Supervisión**. Aparece una página en la que se ven todos los pings actuales.

El separador **Supervisión** solo se puede ver si hay al menos un supervisor configurado.
{:note}

## Adición de un supervisor
{: #adding-a-monitor}

1. En el menú **Dispositivos**, seleccione **Lista de dispositivos**.
2. Pulse el nombre de dispositivo para acceder al dispositivo.
3. Pulse el separador **Supervisión** y seleccione **Gestionar supervisores**.
4. Seleccione **Añadir supervisor**.
5. Seleccione la dirección IP que desea supervisar en la lista **Dirección IP** y el tipo de supervisor en el campo **Tipo de supervisor**. 
6. Configure las opciones de notificación. En el campo **¿Notificar?** seleccione **Notificar a los usuarios** para informar a los usuarios sobre los problemas o **No hacer nada** para omitir la notificación a los usuarios.
7. Seleccione el intervalo de tiempo para la notificación al usuario en el campo **Espera de notificación**.
8. Pulse **Añadir supervisor** para añadir el supervisor al dispositivo. El nuevo supervisor aparece en la sección **Editar supervisores existentes**.

## Edición de un supervisor existente
{: #editing-an-exisiting-monitor}

1. En el menú **Dispositivos**, seleccione **Lista de dispositivos**.
2. Pulse el nombre de dispositivo para acceder al dispositivo.
3. Pulse el separador **Supervisión** y seleccione **Gestionar supervisores**.
4. En la sección **Editar supervisores existentes**, pulse cualquiera de los detalles del supervisor para editar el supervisor.
5. Puede actualizar cualquiera de los siguientes campos: **Tipo de supervisor, Notificar** o **Espera de notificación**.
6. Pulse **Actualizar** para actualizar los detalles.

## Eliminación de un supervisor
{: #removing-a-monitor}

1. En el menú **Dispositivos**, seleccione **Lista de dispositivos**.
2. Pulse el nombre de dispositivo para acceder al dispositivo.
3. Pulse el separador **Supervisión** y seleccione **Gestionar supervisores**.
4. En la sección **Editar supervisores existentes**, pulse el icono **Eliminar** en los detalles del supervisor.
5. Seleccione **Sí** para eliminar el supervisor.

## Siguientes pasos

- Si se añade un nuevo supervisor, el supervisor aparece en el separador **Supervisión**. El supervisor envía un ping al dispositivo cada 5 minutos, esperando una respuesta basada en el tipo de ping seleccionado. Si no se recibe la respuesta esperada, se envía un correo electrónico a la dirección de correo electrónico de notificación correspondiente a la cuenta en el intervalo de tiempo especificado, si se ha seleccionado notificación.
- Si se edita un supervisor, este continúa funcionando según lo especificado en los detalles del supervisor. Si se modifica el tipo, cambia el intervalo de tiempo para recibir el ping esperado. Si se han cambiado las opciones de notificación, la forma en que se notifica a los usuarios de un intento fallido se modifica en función de las nuevas selecciones. El supervisor sigue estando accesible desde el separador **Supervisión**.
- Si se elimina un supervisor, este deja de funcionar para el dispositivo. Toda la supervisión asociada con el supervisor eliminado se detiene y el supervisor deja de aparecer en el separador **Supervisión**.

