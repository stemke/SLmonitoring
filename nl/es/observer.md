Un administrador puede obtener una vista holística del estado actual y pasado de su dispositivo en un mismo lugar.

Casos de usuarios:

    Cualquier usuario puede alternar rápidamente entre los separadores "Ancho de banda" y "Uso" entre su vista existente y la versión beta de observador (solo BETA)

    Cualquier usuario puede proporcionar comentarios sobre su experiencia en la versión beta de observador a través del portal de control (solo BETA)

    Cualquier usuario puede acceder a la publicación del blog para obtener más información acerca de nuestro trabajo en la versión de observador de la experiencia beta (solo BETA)

    A los usuarios se les asigna un lugar en el que pueden almacenar y ver métricas de recursos de la infraestructura correspondientes a servidores virtuales:

    1. Utilización de CPU, %, por núcleo virtual

    2. Red pública, entrada/salida, bytes y paquetes

    3. Red privada, entrada/salida, bytes y paquetes

    4. Utilización de memoria, %

    5. Lectura de disco, bytes y operaciones

    6. Escritura en disco, bytes y operaciones

    7. Errores de transmisión, entrada/salida, recuento

    8. Latencia de disco, ms, lectura y escritura

    9. Utilización de disco local, % y bytes utilizados y total de bytes disponibles


    Los usuarios de dispositivos nativos podrán ver las métricas siguientes:

    1. Utilización de CPU, %, por núcleo virtual

    2. Red pública, entrada/salida, bytes y paquetes

    3. Red privada, entrada/salida, bytes y paquetes

    4. Utilización de memoria, %

    5. Lectura de disco, bytes y operaciones

    6. Escritura en disco, bytes y operaciones

    7. Errores de transmisión, entrada/salida, recuento

    8. Latencia de disco, ms, lectura y escritura

    9. Utilización de disco local, % y bytes utilizados y total de bytes disponibles

    10. Alertas de RAID, 0/1

    11. Temperatura del núcleo, grados F

    Cualquier administrador puede ver el historial de alarmas y métricas en una única vista sin tener que realizar ningún análisis de registro (parecido al número 60)

    Un gestor puede comprender el estado general de su dispositivo sin necesidad de que se lo aclaren sus equipos de administración.

    Cualquier usuario puede abrir el archivo syslog más reciente de un dispositivo sin utilizar la línea de mandatos (parecido al número 35)

    Cualquier usuario puede ver y explorar datos de métricas de serie temporal en un conjunto de diagramas interactivos.

    Cualquier usuario puede ver y obtener una visión general del historial de alertas.

    Cualquier usuario puede marcar sucesos como "abiertos" o "cerrados".

    No es necesario que los usuarios creen manualmente un suceso cuando se activa una alarma.

    No es necesario que los usuarios asignen manualmente un nivel de gravedad de "aviso" o "error" aparte de los valores de alarma.

    Cualquier usuario puede recopilar métricas a nivel de sistema y de aplicación mediante los agentes collectD para los procesos de supervisión, apache, tomcat, MSSQL, MySQL y respuestas de URL.

    Un administrador puede enviar datos de métricas personalizados al servicio de supervisión de forma automática.

    Cualquier usuario puede utilizar las métricas del sistema, de la aplicación o personalizadas de la misma manera que las métricas de hipervisor: gráficos, paneles de control, alarmas, notificaciones, respuestas automáticas, plantillas, etc.



Ventaja 2: un administrador puede comprender y comenzar a solucionar un incidente en 90 segundos

Casos de usuarios:

    Cualquier administrador puede suscribirse a las alertas sin recibir una avalancha de falsos positivos.

    Cualquier administrador puede recibir alertas a través de su canal de comunicación principal en un plazo de un minuto desde que se activa el suceso.

    Los ingenieros de fiabilidad pueden entender la causa de una alerta de incidencias basándose en el mensaje de la propia alerta.

    Cualquier administrador puede consultar las métricas de uso recientes en cualquier dispositivo con un alto grado de precisión.

    Cualquier administrador puede buscar la información exacta que necesita en menos de 10 segundos.

    Un usuario que no sea administrador puede resolver una incidencia que se haya escalado con menos de tres mensajes del equipo de soporte de SL

    Cualquier usuario puede especificar una condición para alertar de cualquier métrica que esté disponible (default, collectD o custom).

    Cualquier usuario puede especificar una condición basada en un valor promedio, un valor acumulado (suma), un valor mínimo o un valor máximo de cualquier métrica.

    Cualquier usuario puede especificar una condición con la calificación "mayor que" o "menor que".

    Cualquier usuario puede especificar el número de periodos consecutivos en que se debe cumplir una condición, así como la duración del periodo, de 30 segundos o 5 minutos, antes de que se active una alarma: "si se produce X durante 2 periodos consecutivos de 30 segundos, entonces se activa la alarma"

    Cualquier usuario puede especificar varias condiciones para una sola alarma: "si sucede esto Y esto Y esto, entonces se activa la alarma".

    Cualquier usuario puede especificar un nombre personalizado para la alarma.

    Se puede informar a cualquier usuario de las alertas con indicaciones de hora, nombre de la alarma y condiciones que se han cumplido para que se activara la alarma.

    Después de que se active una alarma, ningún usuario recibirá alertas adicionales de la misma regla en el mismo dispositivo hasta que se haya "cerrado" la alarma inicial.

    Regla de alarma de ejemplo: si la utilización media de CPU es superior al 80% durante 2 periodos consecutivos de 5 minutos Y la suma de entradas de red es superior a 50 GB durante 1 periodo consecutivo de 5 minutos, se activa una alarma y se crea un suceso (suponiendo que las alarmas anteriores de esta regla se hayan cerrado)

    Un administrador puede especificar 1 o varias direcciones de correo electrónico para notificar a cualquier usuario.

    Un administrador puede especificar 1 o varios números de teléfono de SMS para notificar a cualquier usuario.

    Un administrador puede especificar 1 o varios URL para los webhooks que enviar.

    Un administrador puede especificar un grupo de Pagerduty para notificar a los usuarios.

    Un administrador puede especificar si el servidor se debe rearrancar o concluir cuando se active la alarma.

    Un administrador puede especificar un intervalo de 30 segundos o de 5 minutos para la supervisión de red de cualquier protocolo soportado

    Un administrador puede implementar comprobaciones de ping de host (ICMP)

    Un administrador puede implementar comprobaciones de puertos TCP para diversos protocolos: DNS, DNS custom, FTP, HTTP, HTTP personalizado, HTTPS, IMAP, LDAP, NNTP, POP, SMTP, SSH, TCP personalizado, TELNET, UDP SIP (el soporte para estos protocolos se ofrece en la oferta SL TCP actual)

    Un administrador puede implementar una comprobación de puertos TCP para el protocolo SNMP (no recibe soporte actualmente en la oferta de SL existente)

    Un administrador puede especificar el umbral para el tiempo de respuesta para que una operación se clasifique como correcta o errónea

    Un administrador puede especificar el número de errores consecutivos de un ping de host o una comprobación de puertos TCP antes de que se active una alarma.

    Un administrador puede implementar las mismas opciones de notificación y respuesta automática de las alarmas de supervisión de red que las alarmas basadas en métricas (correo electrónico, SMS, webhook, PagerDuty, rearranque, cierre)

    Un administrador puede especificar el nivel de gravedad de "aviso" o "error" para las alarmas de supervisión tanto de métricas como de red.



Ventaja 3: cualquier usuario puede configurar la supervisión de cualquier dispositivo y dedicar menos de 90 segundos a tomar decisiones sobre configuración (parecido al número 59)

Casos de usuarios:

    Un usuario que no sea administrador puede realizar una configuración básica de su sistema de supervisión utilizando únicamente la interfaz y la documentación.

    Un administrador puede configurar una supervisión que se ajuste a sus necesidades específicas seleccionando configuraciones guardadas o empaquetadas previamente, sin pasar por el proceso de configuración manual (parecido al número 58)

    Un administrador puede configurar una supervisión que se ajuste a sus necesidades específicas editando y guardando manualmente una configuración y luego aplicándola al número de dispositivos que desee.

    Un administrador puede configurar alertas en varios dispositivos con un mínimo esfuerzo de repetición.

    Cualquier usuario puede exportar datos específicos de tiempo y de métrica a un archivo CSV.

    Un administrador o gestor puede configurar una ventana de mantenimiento durante la cual no se enviarán notificaciones cuando se activen alarmas.

    Cualquier usuario establecido puede comprender y aplicar las configuraciones guardadas (parecido al número 41)

    Cualquier usuario nuevo puede comprender y aplicar las configuraciones empaquetadas (parecido al número 34 y 32)

    Un usuario que no sea administrador puede obtener soporte para configurar la supervisión sin rellenar una incidencia de soporte.

    Cualquier cliente puede solicitar supervisión para cualquier dispositivo sin tener conocimientos de experto (parecido al número 63 y 43)

    Todos los clientes tienen una experiencia unificada y previsible para solicitar la supervisión de cualquier dispositivo (parecido al número 40)

    Cualquier usuario puede integrar su dispositivo con un servicio de un tercero sin rellenar una incidencia de soporte.

    No es necesario que los usuarios creen manualmente una alarma para alertas de "aviso" del ciclo de vida: creación, arranque, cierre.

    Cualquier usuario técnico puede acceder a toda la funcionalidad del observador a través de la misma API que se utiliza para el resto del servicio de supervisión.

    IBM puede restringir el acceso de las cuentas a determinadas características/rendimiento con la versión gratuita tal como se define en la visión general del observador sobre el nivel gratuito frente al de pago.

    Cualquier cliente puede actualizar de la versión gratuita a la versión de pago desde el separador de supervisión.

    Cualquier cliente puede actualizar o degradar entre las versiones de pago o gratuita en el área de gestión de cuentas.

    Cualquier usuario con la versión gratuita puede ver las opciones que tendría si actualizara, pero de una forma que indica por qué no están disponibles

    Si un usuario intenta realizar una acción que requeriría que se realizara una actualización, debería ver un mensaje que explica que tiene que actualizar y que muestra una alternativa, si existe (por ejemplo, "ya tiene el número máximo de alarmas para la versión gratuita. Actualice o suprima una alarma para crear una nueva regla").


