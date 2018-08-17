---
copyright:
  years: 2018
lastupdated: "2018-05-18"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Creación y gestión de notificaciones de supervisión (Beta)
Una notificación describe el método y los detalles que se utilizan para la notificación cuando se activa una alerta. Por ejemplo, para obtener una notificación de aviso y una notificación de error para una métrica, defina una regla que supervise el umbral de aviso y defina una regla que supervise el umbral de error.
{:shortdesc} 

## Crear una notificación
 
 1. Una vez que se haya unido a la versión beta, seleccione **Dispositivos -> Supervisión**. 
 2. Pulse el separador **Notificaciones**.
 3. Pulse **Crear notificación**.
 4. Escriba la información de la nueva notificación. 

<table>
  <caption>Detalles de notificación por correo electrónico</caption>
  <tr>
     <th>Campo</th>
     <th>Descripción</th>
  </tr>
  <tr>
    <td>Nombre</td>
    <td>Un identificador exclusivo de la notificación. Este campo es obligatorio.</td>
  </tr>
  <tr>
    <td>Tipo</td>
    <td>Seleccione: **Email**</td>
  </tr>
  <tr>
    <td>Dirección de correo electrónico</td>
    <td>Escriba la dirección de correo electrónico del destinatario.</td>
  </tr>
</table>

<table>
  <caption>Detalles de notificación por webhook</caption>
  <tr>
     <th>Campo</th>
     <th>Descripción</th>
  </tr>
  <tr>
    <td>Nombre</td>
    <td>Un identificador exclusivo de la notificación. Este campo es obligatorio.</td>
  </tr>
  <tr>
    <td>Tipo</td>
    <td>Seleccione: **Webhook**</td>
  </tr>
  <tr>
    <td>URL de Webhook</td>
    <td>Escriba el URL en el que se debe realizar la solicitud POST.</td>
  </tr>
  <tr>
  <td>Verificar certificados</td>
    <td>Seleccione esta opción para verificar los certificados.</td>
  </tr>
  <tr>
    <td>Cabeceras de webhook</td>
    <td>Especifique las cabeceras.</td>
  </tr>
  <tr>
    <td>Parámetros de consulta de webhook</td>
    <td>Escriba los parámetros de consulta.</td>
  </tr>
</table>

<table>
  <caption>Detalles de notificación por PagerDuty</caption>
  <tr>
     <th>Campo</th>
     <th>Descripción</th>
  </tr>
  <tr>
    <td>Nombre</td>
    <td>Un identificador exclusivo de la notificación. Este campo es obligatorio.</td>
  </tr>
  <tr>
    <td>Tipo</td>
    <td>Seleccione: **Pager duty**</td>
  </tr>
  <tr>
    <td>Clave de API</td>
    <td>Escriba la clave de API correspondiente a la notificación por PagerDuty.</td>
  </tr>
</table>


5. Pulse **Aceptar** para crear las nuevas notificaciones con el valor que ha especificado.

## Editar una notificación
 1. Una vez que se haya unido a la versión beta, seleccione **Dispositivos -> Supervisión**. 
 2. Pulse el separador **Notificaciones**.
3. Pulse **Acciones->Editar notificación**.
4. Edite cualquiera de los detalles de la notificación.
5. Pulse **Aceptar** para aceptar los cambios.

## Suprimir una notificación
1. Una vez que se haya unido a la versión beta, seleccione **Dispositivos -> Supervisión**. 
2. Pulse el separador **Notificaciones**.
3. Pulse **Acciones->Suprimir notificación**.
4. Pulse **Suprimir** para confirmar su elección.

## Añadir varias notificaciones a un dispositivo
1. Seleccione **Infraestructura->Lista de dispositivos>*Nombre de dispositivo*** para acceder a los detalles del dispositivo.
2. Pulse **Acciones->Gestionar notificaciones**.
4. Pulse para asignar o eliminar notificaciones correspondientes al dispositivo.

