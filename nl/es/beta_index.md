---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# Iniciación a IBM Cloud Monitoring (Beta)
{: #gettingstartedbeta}

Esta aplicación de supervisión beta, que se basa en el servicio de supervisión de {{site.data.keyword.BluSoftlayer_full}}, está disponible para los servidores virtuales y nativos. Para ver las actualizaciones sobre el desarrollo de este programa Beta, consulte el [blog de IBM Cloud ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}.
{:shortdesc}

## Requisitos previos

Para participar en este programa Beta, debe cumplir con estos requisitos.
1. La cuenta de SoftLayer debe estar enlazada a una cuenta de IBM Cloud con autenticación de IBMid. Para enlazar una cuenta, el usuario maestro de la cuenta de SoftLayer debe iniciar una sesión en [{{site.data.keyword.slportal}} ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com){: new_window} y desde el menú **Cuenta**, pulse **Enlazar una cuenta de Bluemix**.
2. Para poder ver la versión Beta, cada usuario debe estar enlazado a un ID de IBM. Para obtener más información, consulte [Enlace de cuentas de usuario de IBMid](/docs/account?topic=account-unifyingaccounts#link_customer_accounts).
3. Para poder ver la versión Beta, cada usuario debe tener acceso al servicio de supervisión de IBM Cloud.
   1. Desde la consola de [IBM Cloud ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://console.bluemix.net){: new_window}, seleccione **Gestionar -> Cuenta -> Usuarios**.
   2. Invite al usuario a la cuenta o seleccione el usuario en la lista.
   3. Seleccione **Asignar acceso a recursos** para el usuario.
   4. En **Servicio**, seleccione **Servicio de supervisión de IBM Cloud**.
   5. Seleccione el **Rol** que desea asignar al usuario para todas las regiones.

Si no cumple estos requisitos previos, no podrá acceder a la supervisión Beta en este momento.


## Cómo unirse a la versión beta

Siga estos pasos para empezar a utilizar el programa Beta de supervisión. Unirse a la versión Beta habilita el servicio para todos los servidores virtuales y nativos aptos de su cuenta. El hecho de pulsar Unir no afecta a los datos ni al servicio de supervisión de Nimsoft existentes.
1. (Solo servidor nativo) [Instale el agente de supervisión en el servidor nativo](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-).
<table>
   <CAPTION>Tabla 1. Elija una ubicación de inicio de sesión</CAPTION>
   <THEAD>
   <TR>
   <th>Si desea unirse con...</th>
   <th>Entonces...</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>Catálogo de IBM Cloud</td>
   <td>
   <ol>
   <li>Abra una nueva ventana del navegador y escriba <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>.</li>
   <li>Pulse el enlace <b> Iniciar sesión</b>. </li>
   <li>Escriba su correo electrónico o IBMid y pulse <b>Continuar</b>.</li>
   <li>Escriba su contraseña y pulse <b>Iniciar sesión</b>.</li>
   <li>Seleccione **Infraestructura->Lista de dispositivos>*Nombre de dispositivo*** para acceder a los detalles del dispositivo.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>Portal de clientes</td>
   <td>
   <ol>
   <li>Abra una nueva ventana del navegador y escriba <a href="https://control.softlayer.com">https://control.softlayer.com</a>.</li>
   <li>Escriba el nombre de usuario y la contraseña y pulse <b> Iniciar sesión</b>. O bien, pulse <b>Iniciar sesión con IBMid</b>. A continuación, escriba su correo electrónico o IBMid y pulse <b>Continuar</b>. Escriba su contraseña y pulse <b>Iniciar sesión</b>. Se abrirá la página principal del {{site.data.keyword.slportal}}.</li>
     <li>En **Dispositivos**, pulse el **Nombre de dispositivo** para acceder a los detalles del dispositivo.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. Seleccione **Dispositivos > Supervisión**. Pulse **Unirse a la versión beta** para ver los separadores de políticas del sistema y notificaciones de la versión beta.

## Siguientes pasos
1. Revise los detalles de las [métricas](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-) recopiladas.
2. [Cree o gestione](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-) una notificación del supervisor.
3. [Cree o gestione](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-) una política del sistema.
4. [Vea las alertas](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-).
5. Revise los datos actualmente disponibles del gráfico de supervisión de la versión Beta para un dispositivo seleccionado.

|              Métricas                                      |  Descripción                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|Utilización de CPU                                            |   Ver el % de utilización de CPU para cada núcleo y un promedio de los núcleos. Pulse cada métrica para activar o desactivar los datos en el gráfico.
|Red pública                                             |   Ver los datos de entrada y de salida correspondientes a la red pública. Pulse cada métrica para activar o desactivar los datos en el gráfico.       |
|Red privada                                            |   Ver los datos de entrada y de salida correspondientes a la red privada. Pulse cada métrica para activar o desactivar los datos en el gráfico.           |
|Utilización de memoria    | Ver el % de utilización de memoria del servidor     |
|Uso de disco    | Ver la cantidad media de datos que se leen o escriben en disco en bytes o la latencia de disco. Pulse cada métrica para activar o desactivar los datos en el gráfico.    |
|Temperatura                                                 |Ver la temperatura del dispositivo nativo en grados Celsius. Estos datos no están disponibles para todos los dispositivos.
{: caption="Tabla 1. Métricas de Beta" caption-side="top"}   

## Limitaciones
Si se suprime un dispositivo, las políticas de supervisión asociadas no se suprimen. Tenga en cuenta que debe suprimir manualmente el dispositivo para estas políticas.

Los datos de métricas solo están disponibles durante 15 días.

Solo pueden existir 10 políticas de supervisión simultáneamente. Sin embargo, una política se puede aplicar a varios dispositivos.

## Resolución de problemas
Para ver algunas métricas, como la utilización de memoria, se necesitan las herramientas Xen en el servidor. Para obtener información sobre cómo instalar las herramientas Xen, consulte [Preparación e importación de imágenes](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images).

## Comentarios
Para proporcionar comentarios sobre esta versión Beta, seleccione **Dispositivos -> Supervisión** o la página de detalles del dispositivo y pulse **Dejar comentarios** para cumplimentar una breve encuesta. Para salir de la versión Beta y volver a la vista estándar, pulse el enlace **Abandonar Beta** en la parte inferior de la página **Dispositivos -> Supervisión**.
