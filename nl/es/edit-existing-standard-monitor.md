---

copyright:
  years: 2014, 2018
lastupdated: "2018-10-30"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Edición de un supervisor existente
Después de que se añada un supervisor a un dispositivo, puede modificarlo o eliminarlo cuando lo desee. Las modificaciones en supervisores permiten realizar cambios en las opciones de tipo y de modificación, mientras que la eliminación de un supervisor cancela el supervisor por completo. Siga estos pasos para editar un supervisor existente.

1. En la página **Supervisores** bajo la cabecera **Editar supervisores existentes**, pulse cualquiera de los detalles del supervisor para abrir el supervisor para editarlo.

2. Modifique los **Detalles del supervisor** que desee. Consulte la tabla para obtener más detalles sobre cada campo editable.

|Campo|Detalles|Acción|
|---|---|---|
|Tipo de supervisor|El intervalo de tiempo en el que se espera recibir una respuesta del dispositivo. El sistema toma como valor predeterminado un ping de servicio. Un ping lento espera una respuesta durante 5 segundos, lo que permite que los servidores que están optimizados para tareas que no son de red tengan más tiempo para procesar la solicitud. Un ping de servicio emite un ping cada 5 minutos y espera una respuesta de eco en un plazo de 1 segundo. Si se ha perdido más de un ping, se emite una alerta.|Seleccione la opción **Ping lento** o la opción **Ping de servicio**.|
|Notificar| Los usuarios notificados reciben notificaciones automáticas cuando un dispositivo no responde a un ping en el tiempo de respuesta asignado. Para recibir notificación, un usuario debe estar en la cuenta asociada al dispositivo.|Para añadir un usuario, seleccione el nuevo **Usuario notificado** y pulse **Añadir usuario**. Para eliminar un usuario, pulse el icono **Eliminar** situado
junto al usuario notificado existente y pulse **Sí** para confirmar la acción.|
|Espera de notificación|El intervalo de tiempo que el sistema espera para enviar una notificación cuando el dispositivo no ha respondido a una operación ping. Hay varios tiempos de espera disponibles. **Nota:** los detalles de notificación no son necesarios cuando no se ha seleccionado ningún usuario para la notificación. |Seleccione el tiempo de espera que necesite.|

3. Pulse **Actualizar** para aplicar los cambios al supervisor. Pulse **Cancelar** si desea cancelar la acción.

## Siguientes pasos

Si se edita un supervisor, este continúa funcionando según lo especificado en los detalles del supervisor. Si se modifica el tipo, cambia el intervalo de tiempo para recibir el ping esperado. Si las opciones de notificación cambian, la modalidad de notificación se modifica en función de las nuevas selecciones. El supervisor sigue estando accesible desde el separador de supervisión.
