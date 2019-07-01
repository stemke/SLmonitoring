---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configuración de un informe de agente de Nimsoft Monitoring
{: #configuring-a-nimsoft-monitoring-agent-report}

## Antes de empezar

Primero, navegue hasta el menú del dispositivo y asegúrese de tener los permisos de cuenta correctos para completar las tareas.

* Navegue hasta el menú del dispositivo de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Asegúrese de que tiene los permisos de cuenta y el acceso de dispositivo necesarios. Solo el propietario de la cuenta, o un usuario con el permiso de la infraestructura clásica **Gestionar usuarios**, puede ajustar los permisos.

Para obtener más información sobre permisos, consulte [Permisos de la infraestructura clásica](/docs/iam?topic=iam-infrapermission#infrapermission) y [Gestión del acceso a dispositivos](/docs/vsi?topic=virtual-servers-managing-device-access).

## Configuración de un informe de agente de Nimsoft Monitoring
{: #configuring-nimsoft-monitoring-agent-report-steps}

Siga los siguientes pasos para configurar un informe de agente de Nimsoft Monitoring.

1. En el menú **Dispositivos**, seleccione **Supervisión**.
2. En la pantalla **Supervisión**, seleccione **Configurar informes de agente** en el menú desplegable **Acciones** en la columna **Avanzado**.
3. Seleccione el agente que desea configurar en la lista desplegable **Agentes**.
  
  Los agentes disponibles varían según el dispositivo y dependen del paquete de supervisión aplicado al dispositivo.
  {:note}

4. Seleccione la sección que desea configurar en la lista desplegable **Secciones**. Si selecciona una sección que contiene perfiles, aparece otra lista desplegable. En dicha lista, seleccione un **perfil existente** en la lista desplegable **Perfiles**. Para añadir una nueva configuración, seleccione **Añadir configuración de agente...** en la lista desplegable **Perfiles**.

5. Complete cada campo de la sección **Métricas generales e información**, si es necesario.
  
  Los campos obligatorios se indican mediante un asterisco rojo (*). No todos los agentes, secciones o perfiles contienen esta sección.
  {:note}

6. Pulse el recuadro de selección **Métrica** para que cada métrica se desee incluir en el informe en la sección **Seleccionar métricas sobre las que informar**, si procede.

7. Pulse el recuadro de selección **Alarma** para cada alarma que desee activar para el agente en **Alarmas de métricas**.

  No todas las alarmas de esta sección están vinculadas a una métrica específica. Se envían alarmas a cada dirección de correo electrónico asociada a la sección **Suscriptores de alarma** para el agente.
  {:note}

7. Pulse **Guardar** para guardar la configuración. Pulse **Cancelar** si desea cancelar la acción.
  
  El botón **Guardar** está inhabilitado hasta que se realiza un cambio en la configuración actual.
  {:note}

## Siguientes pasos

Después de guardar correctamente la configuración, aparecerá un mensaje de confirmación. Si la configuración no se ha realizado correctamente, se mostrará un mensaje de error con detalles sobre el error que se ha producido y sobre cómo solucionarlo. Para volver a configurar los agentes en cualquier momento, repita estos pasos.
