---

copyright:
  years: 2017
lastupdated: "2017-09-28"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Visualización y gestión de supervisores
{: viewing-and-managing-monitors}

La supervisión de un dispositivo permite a los usuarios iniciar operaciones ping de servicio y lentas para asegurarse de que el dispositivo está en línea y responde.
{:shortdesc}

Si no se recibe un eco durante el periodo de tiempo asignado (1 segundos para operaciones ping de servicio, 5 segundos para operaciones ping lentas), se envía una alerta a la dirección de correo electrónico especificada en la cuenta. El valor **Up (activo)** en el campo **Estado** indica que se ha recibido un eco y **Down (inactivo)** indica que no se ha recibido. Si dispone de un supervisor básico configurado, siga estos pasos para ver y gestionar la supervisión de un dispositivo.

   <table>
   <CAPTION>Tabla 1. Ver y gestionar la supervisión de un dispositivo</CAPTION>
   <THEAD>
   <TR>
   <th>Si la acción que se va a emprender es...</th>
   <th>Entonces...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Ver supervisores</td>
   <td>
   <ol>
   <li>En la lista de dispositivos, pulse el <b>Nombre de dispositivo</b> para acceder al dispositivo.</li>
   <li>Pulse el separador <b>Supervisión</b>. Aparece una página en la que se ven todos los pings actuales. (El separador <b>Supervisión</b> solo se puede ver si hay al menos un supervisor configurado.)</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Añadir un supervisor</td>
   <td>
   <ol>
   <li>En el separador <b>Supervisión</b> de la página Detalles del dispositivo, pulse <b>Gestionar supervisores</b> en la parte derecha de la página para gestionar los supervisores asociados a este dispositivo.</li>
   <li>En la página Supervisores, pulse el separador <b>Añadir supervisor</b>.</li>
   <li>Seleccione la dirección IP que desea supervisar en la lista <b>Dirección IP</b>.</li>
   <li>Seleccione el tipo de supervisor en la lista <b>Tipo de supervisor</b>.</li>
   <li>Configure las opciones de notificación. En la lista <b>¿Notificar?</b>, seleccione <b>Notificar a los usuarios</b> para informar a los usuarios sobre los problemas o <b>No hacer nada</b> para omitir la notificación a los usuarios.</li>
   <li>Seleccione el intervalo de tiempo para la notificación al usuario en la lista <b>Espera de notificación</b>.</li>
   <li>Pulse <b>Añadir supervisor</b> para añadir el supervisor para el dispositivo. El nuevo supervisor aparece en la sección <b>Editar supervisores existentes</b> de la pantalla.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Editar un supervisor existente</td>
   <td>
   <ol>
   <li>En la página Supervisores, bajo la cabecera <b>Editar supervisores existentes</b>, pulse cualquiera de los detalles del supervisor para editar el supervisor.</li>
   <li>Puede actualizar cualquiera de los siguientes campos: Tipo de supervisor, Notificar, Espera de notificación.</li>
   <li>Pulse <b>Actualizar</b> para actualizar los detalles. Pulse <b>Cancelar</b> para cancelar la edición.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Eliminar un supervisor</td>
   <td>
   <ol>
   <li>En la página Supervisores, bajo la cabecera <b>Editar supervisores existentes</b>, pulse el icono Eliminar que hay junto a los detalles del supervisor.</li>
   <li>Pulse <b>Sí</b> para eliminar el supervisor. Pulse <b>No</b> para
cancelar la acción.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
   </table>

## Siguientes pasos

- Si se añade un nuevo supervisor, el supervisor aparece en el separador **Supervisión**. El supervisor envía un ping al dispositivo cada 5 minutos, esperando una respuesta basada en el tipo de ping seleccionado. Si no se recibe la respuesta esperada, se envía un correo electrónico a la dirección de correo electrónico de notificación correspondiente a la cuenta en el intervalo de tiempo especificado, si se ha seleccionado notificación.
- Si se edita un supervisor, este continúa funcionando según lo especificado en los detalles del supervisor. Si se modifica el tipo, cambia el intervalo de tiempo para recibir el ping esperado. Si se han cambiado las opciones de notificación, la forma en que se notifica a los usuarios de un intento fallido se modifica en función de las nuevas selecciones. El supervisor sigue estando accesible desde el separador **Supervisión**.
- Si se elimina un supervisor, este deja de funcionar para el dispositivo. Toda la supervisión asociada con el supervisor eliminado se detiene y el supervisor deja de aparecer en el separador **Supervisión**.
