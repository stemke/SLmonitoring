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

# Visualización de un informe de agente para Nimsoft Monitoring
{: #viewing-an-agent-report-for-nimsoft-monitoring}

Los detalles de supervisión de Nimsoft Monitoring están disponibles en los informes de agente, que proporcionan los detalles específicos sobre la forma en que se ha configurado el agente. 
{:shortdesc}

## Antes de empezar
Primero, navegue hasta el menú del dispositivo y asegúrese de tener los permisos de cuenta correctos para completar las tareas.

* Navegue hasta el menú del dispositivo de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices).
* Asegúrese de que tiene los permisos de cuenta y el acceso de dispositivo necesarios. Solo el propietario de la cuenta, o un usuario con el permiso de la infraestructura clásica **Gestionar usuarios**, puede ajustar los permisos.

Para obtener más información sobre permisos, consulte [Permisos de la infraestructura clásica](/docs/iam?topic=iam-infrapermission#infrapermission) y [Gestión del acceso a dispositivos](/docs/vsi?topic=virtual-servers-managing-device-access).

## Visualización de un informe de agente para Nimsoft Monitoring
{: #viewing-agent-report-nimsoft-monitoring-steps}

Siga estos pasos para ver un informe de agente para Nimsoft Monitoring.

1. En la página **Supervisión**, seleccione **Ver informes de agente** en el menú **Acciones**.
2. Seleccione el agente que desea ver en la lista **Agentes**.

  Los agentes disponibles varían según el dispositivo y dependen del paquete de supervisión aplicado al dispositivo.
  {:note}
  
3. Complete todas las secciones restantes, incluidas una o varias de las acciones siguientes:

  Cada agente es diferente y no incluye cada sección o métrica. Las opciones disponibles en esta pantalla dependen de las opciones de configuración disponibles para cada agente.
  {:note}
  
  * Seleccione el informe de sección en la lista **Secciones**.
  * Seleccione el periodo de tiempo para el informe en la lista **Ver por**.
  * Pulse el recuadro de selección correspondiente a cada métrica que desee incluir en el informe en la sección **Seleccionar métricas sobre las que informar**.
    
    En el mismo gráfico solo aparecen las métricas parecidas. Si se eligen métricas en conflicto, se produce un error después de solicitar el gráfico.
    {:note}
4. Pulse **Dibujar gráfico** para dibujar el gráfico.

## Siguientes pasos

Después de dibujar el gráfico para el informe de agente, si quiere volver a dibujar el gráfico en cualquier momento para ver las distintas métricas repita estos pasos. No hay límite en el número de informes de agente que se pueden generar dentro de un periodo de tiempo establecido.
