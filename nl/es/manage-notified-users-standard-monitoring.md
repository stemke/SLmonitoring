---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestión de usuarios notificados para la supervisión estándar
{: #managing-notified-users-for-standard-monitoring}

Los usuarios notificados para el servicio de supervisión estándar reciben notificaciones automáticas cuando un dispositivo no responde a un ping en el tiempo de respuesta asignado. Puede añadir o eliminar usuarios notificados en cualquier momento, y los usuarios notificados deben estar en la cuenta asociada con el dispositivo para recibir una notificación. Siga estos pasos para gestionar los usuarios notificados para el servicio de supervisión estándar.
{:shortdesc}

## Antes de empezar
Primero, navegue hasta el menú del dispositivo y asegúrese de tener los permisos de cuenta correctos para completar las tareas.

* Navegue hasta el menú del dispositivo de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Asegúrese de que tiene los permisos de cuenta y el acceso de dispositivo necesarios. Solo el propietario de la cuenta, o un usuario con el permiso de la infraestructura clásica **Gestionar usuarios**, puede ajustar los permisos.

Para obtener más información sobre permisos, consulte [Permisos de la infraestructura clásica](/docs/iam?topic=iam-infrapermission#infrapermission) y [Gestión del acceso a dispositivos](/docs/vsi?topic=virtual-servers-managing-device-access).

## Adición de usuarios notificados
{: #adding-notified-users}

Siga los siguientes pasos para añadir usuarios notificados para el servicio de supervisión estándar.
1. En el menú **Dispositivo**, seleccione **Lista de dispositivos**.
2. Pulse el nombre de dispositivo para acceder al dispositivo.
3. Pulse el separador **Supervisión** y seleccione **Gestionar supervisores**.
4. Seleccione **Gestionar usuarios notificados**.
5. En la lista desplegable **Usuarios que notificar**, seleccione el nuevo usuario que desea notificar.
6. Seleccione **Añadir usuario**.

## Eliminación de usuarios notificados
{: #removing-notified-users}

Siga los siguientes pasos para eliminar usuarios notificados para el servicio de supervisión estándar.
1. En el menú **Dispositivo**, seleccione **Lista de dispositivos**.
2. Pulse el nombre de dispositivo para acceder al dispositivo.
3. Pulse el separador **Supervisión** y seleccione **Gestionar supervisores**.
4. Seleccione **Gestionar usuarios notificados**.
5. Pulse el icono **Eliminar** para eliminar el usuario notificado existente y, a continuación, seleccione **Sí** para eliminar el usuario. 

## Siguientes pasos

Si añade un usuario notificado, se notificará al usuario en el caso de que se haya perdido una respuesta de ping. Si ha eliminado un usuario notificado, el usuario dejará de recibir una notificación relacionada con una respuesta de ping que se ha perdido asociada con el dispositivo.
