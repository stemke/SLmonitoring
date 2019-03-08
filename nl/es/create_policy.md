---

copyright:
  years: 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creación y gestión de políticas del sistema (Beta)
Puede crear políticas para activar notificaciones cuando el dispositivo alcance un umbral de supervisión predeterminado. Por ejemplo, puede notificar a los usuarios si el uso medio de CPU del dispositivo alcanza un nivel de aviso o de error. Solo pueden existir 10 políticas de supervisión simultáneamente. Sin embargo, una política se puede aplicar a varios dispositivos.
{:shortdesc}


Siga estos pasos para trabajar con políticas del sistema.
1. Después de unirse a la versión beta, seleccione **Dispositivos -> Supervisión**.
2. Pulse el separador **Políticas del sistema**.

<table>
   <CAPTION>Tabla 1. Crear y gestionar políticas del sistema</CAPTION>
   <THEAD>
   <TR>
   <th>Si la acción que se va a emprender es...</th>
   <th>Entonces...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Crear una política</td>
   <td>
   <ol>
     <li>Pulse <b>Crear notificación</b>.</li>
     <li>Escriba la información correspondiente a la nueva política del sistema.

<table>
  <caption>Detalles de la política del sistema</caption>
  <tr>
     <th>Campo</th>
     <th>Descripción</th>
  </tr>
  <tr>
    <td>Nombre</td>
    <td>Escriba un identificador exclusivo para la nueva política del sistema. Este campo es obligatorio.</td>
  </tr>
  <tr>
    <td>Activador</td>
    <td>Seleccione los detalles que activarán la política del sistema. Puede definir distintos niveles de métricas para avisos y errores. Por ejemplo, <i>Promedio</i>.</td>
  </tr>
   <tr>
    <td>Duración</td>
     <td>Seleccione la duración que debe tener el suceso para que se active la política.</td>
  </tr>
   <tr>
    <td>Dispositivo</td>
    <td>El dispositivo supervisado para la política.</td>
  </tr>
   <tr>
    <td>Notificación predeterminada</td>
    <td>Defina la notificación predeterminada para la política.</td>
  </tr>
</table>
</li>
<li>Pulse <b>Aceptar</b> para aceptar los cambios.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Editar una política</td>
   <td>
   <ol>
     <li>Pulse <b>Editar una política</b>.</li>
    <li>Escriba la información modificada para la política del sistema.

<table>
  <caption>Detalles de la política del sistema</caption>
  <tr>
     <th>Campo</th>
     <th>Descripción</th>
  </tr>
  <tr>
    <td>Nombre</td>
    <td>Escriba un identificador exclusivo para la nueva política del sistema. Este campo es obligatorio</td>
  </tr>
  <tr>
    <td>Activador</td>
    <td>Seleccione los detalles que activarán la política del sistema. Puede definir distintos niveles de métricas para avisos y errores.</td>
  </tr>
   <tr>
    <td>Duración</td>
     <td>Seleccione la duración que debe tener el suceso para que se active la política.</td>
  </tr>
</table>
</li>
<li>Pulse <b>Aceptar</b> para aceptar los cambios.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Eliminar una política</td>
   <td>
   <ol>
     <li>Pulse <b>Acciones->Suprimir política</b>.</li>
     <li>Pulse <b>Suprimir</b> para confirmar su elección.</li>
   </ol>
   </td>
   </tr>
   <tr>
  <td>Asignar dispositivos</td>
  <td>
    <ol>
      <li>Pulse <b>Gestionar dispositivos</b>.</li>
      <li>Seleccione o desmarque los dispositivos que desea asignar a la política.</li>
       <li>Pulse <b>Aceptar</b> para aceptar los cambios.</li>
    </ol>
      </td>
  </tr>
   <tr>
  <td>Duplicar una política</td>
  <td>
    <ol>
      <li>Pulse <b>Acciones->Duplicar política</b>.</li>
      <li>Escriba la información modificada para la nueva política.</li>
       <li>Pulse <b>Aceptar</b> para aceptar los cambios.</li>
    </ol>
      </td>
  </tr>

   </TBODY>
   </table>
