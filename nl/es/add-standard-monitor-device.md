---
copyright:
  years: 1994, 2017
lastupdated: "2017-06-09"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Adición y eliminación de supervisores

<table>
   <CAPTION>Tabla 1. Adición y eliminación de supervisores de dispositivos</CAPTION>
   <THEAD>
   <TR>
   <th>Si la acción que se va a emprender es...</th>
   <th>Entonces...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Añadir un supervisor</td>
   <td>
   <ol>
   <li>En el separador <b>Supervisión</b> de la página Detalles del dispositivo, pulse <b>Gestionar supervisores</b> en la parte derecha de la página para gestionar los supervisores asociados a este dispositivo.</li>
   <li>En la página Supervisores, pulse el separador <b>Añadir supervisor</b>.
   * **Nota:** las direcciones IP públicas y privadas están disponibles para la supervisión. Cada dirección IP está identificada en el separador **Información del servidor**.</li>
   <li>Seleccione la dirección IP que desea supervisar en la lista desplegable <b>Dirección IP</b>.</li>
   <li>Seleccione el tipo de supervisor en la lista desplegable <b>Tipo de supervisor</b>.</li>
   <li>Configure las opciones de notificación. En la lista desplegable <b>¿Notificar?</b>, seleccione <b>Notificar a los usuarios</b> para informar a los usuarios sobre los problemas o <b>No hacer nada</b> para omitir la notificación a los usuarios.</li>
   <li>Seleccione el intervalo de tiempo para la notificación al usuario en la lista desplegable <b>Espera de notificación</b>.</li>
   <li>Pulse <b>Añadir supervisor</b> para añadir el supervisor para el dispositivo. El nuevo supervisor aparece en la sección <b>Editar supervisores existentes</b> de la pantalla.</li>
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

- Si se elimina un supervisor, dejará de funcionar para el dispositivo. Toda la supervisión asociada con el supervisor eliminado se detiene y el supervisor deja de aparecer en el separador Supervisión.
