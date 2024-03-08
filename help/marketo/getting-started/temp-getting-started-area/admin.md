---
description: 'NUEVA ÁREA: Documentos de Marketo: documentación del producto'
title: NUEVA ÁREA
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 3%

---

# NUEVA ÁREA: Lista de comprobación de administración {#new-area-admin-checklist}

Texto de introducción.

## Funciones {#roles}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Funciones</td>
    <td><li>Revise las funciones prediseñadas y confirme qué permisos/acceso tiene cada función.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Crear una función nueva</a> o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">editar los roles</a> en función de las necesidades de su organización y de la frecuencia con la que los usuarios inicien sesión.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Asignar usuarios a las funciones adecuadas</a>.</li>
    <li>Después de asignar las funciones de los usuarios, revise el número de usuarios por función.</li>  <li>Implemente una función única para cada usuario de API para facilitar la resolución de problemas.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentación</td>
    <td>Defina usuarios y funciones para su organización. <br>Defina el proceso para agregar un nuevo usuario/administrador.</td>
    <td></td>
  </tr>
  <tr>
    <td>Zona protegida (si corresponde)</td>
    <td>Revise las categorías anteriores para su zona protegida si tiene una.</td>
    <td></td>
  </tr>
</tbody>
</table>

## Espacios de trabajo y particiones {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espacios de trabajo y particiones </td>
    <td><li>Determinar el número de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> workspaces</a> y/o particiones que su organización necesita tener y <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">cuántos usuarios tienen acceso a cada espacio de trabajo.</a></li>
    <li>Defina el propósito principal de cada espacio de trabajo y partición.</li>
    <li>Definir la relación entre los espacios de trabajo y las particiones.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentación</td>
    <td><li>Documente cómo se definen los espacios de trabajo y cómo se relacionan con las particiones de la base de datos (es decir, un espacio de trabajo global que vea a todos, en comparación con los sectores empresariales).</li>
    <li>Importe los registros nuevos a la partición apropiada.</li>
    <li>Defina el valor en CRM que coloca a los usuarios en la partición apropiada.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Configuración de campañas inteligentes {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Configuración de campañas inteligentes </td>
    <td><li>Añadir un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">restricción en el tamaño de la campaña inteligente</a>, evitando el envío accidental de toda la base de datos.</li>
    <li>Habilitar restricciones de persona para campañas inteligentes</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Configuración del correo electrónico {#email-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Valores predeterminados de correo electrónico</td>
    <td><li>En Dominio de marca, seleccione su dominio y añada su CNAME de correo electrónico. Debe tener el siguiente formato: [EmailTrackingCNAME].[CompanyDomain].com.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Configuración de SPF y DKIM</a> para la entrega de correo electrónico.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Límites de comunicación {#communication-limits}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Límites de comunicación</td>
    <td><li>Lugar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Límites de comunicación</a>.</li>
    <li>Determine si su empresa requiere una política sobre límites de comunicación.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Etiquetas {#tags}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canales</td>
    <td><li>Defina cómo utilizar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">canales</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Etiquetas </td>
    <td><li>Defina cómo utilizar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">etiquetas</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Calendario (si procede) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Puestos del calendario de marketing de problemas</a> para aquellos que necesitan acceso.</li> 
    <li>Configuración de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Calendario</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Administración de bases de datos {#database-management}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administración de campos</td>
    <td><li>Implementar la convención de nombres para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">campos personalizados.</a> Por ejemplo, comience por "MKTO".</li>
    <li>Sea selectivo sobre los campos que sincroniza. Cuantos más campos sincronice, más lento será el ciclo de sincronización.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Bloquear actualizaciones de campos</a> desea que se escriba una vez (es decir, origen del posible cliente original, detalle del origen del posible cliente original, campos de UTM de primer contacto, etc.).</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Actividades personalizadas </td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">Actividades personalizadas</a> que son específicos de su negocio.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Objetos personalizados </td>
    <td><li>Revisar cuántos <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">Objetos personalizados</a> lo necesitas.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Sincronizar esos objetos personalizados con su CRM</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Integraciones {#integrations}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Iniciar sincronización de CRM. Elija entre las siguientes opciones, según el CRM que utilice su compañía: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>Identifique el tipo de acceso que necesita para acceder a su CRM.</li>
    <li>Identifique al administrador de CRM para la resolución de problemas.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Perspectiva de ventas (si corresponde)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">Configurar perspectiva de ventas.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Emita puestos para los usuarios adecuados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">Configuración de la API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">Personalizar las puntuaciones de los posibles clientes.</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>Páginas de destino </td>
    <td>NOTA: ¿Es cliente de Launch Pack? Puede omitir este paso. Su asesor le proporcionará un documento de instrucciones de configuración de TI durante la llamada de inicio. <br>Configure su dominio de página de aterrizaje con una <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> y <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">introducir información de dominio y página</a>. Debe tener el formato siguiente: [LandingPageCNAME].[CompanyDomain].com <br>Elija un CNAME para las páginas de aterrizaje. Algunos ejemplos: <br>* **ir**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br>SUGERENCIA: ¡Utilice una URL corta! Las direcciones URL más cortas son más fáciles de recordar. Sugerimos "ir" como dominio. <br>Agregue código de seguimiento de análisis (por ejemplo, Google Analytics o Adobe Analytics) a las plantillas de página de aterrizaje. </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">Editar configuración de página de aterrizaje</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">NOTA: Si es cliente de Launch Pack, omita este paso. Su asesor le proporcionará las instrucciones de código de Munchkin en su documento de instrucciones de configuración de TI. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">Añadir el código de seguimiento de Munchkin</a> a su sitio web. El código Munchkin puede ser <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">codificado</a> o implementado mediante Google Tag Manager.</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">Añadir el código de seguimiento de Munchkin a su sitio web</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">Seguimiento de posibles clientes</a> </td>
  </tr>
  <tr>
    <td>Servicios web </td>
    <td>Activar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">las restricciones de IP</a> si procede. <br>Determine los usuarios/aplicaciones que pueden hacer lo siguiente <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">Llamadas de API</a> en su instancia. <br>Revise todas las aplicaciones que realizarán llamadas a la API y determine si es necesario un aumento o un recorte para las llamadas a la API.</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">Creación de una Lista de permitidos para el acceso a API basado en IP </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (si procede) </td>
    <td>Para usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>, el canal nativo de participación conversacional de Marketo Engage, seguirá con la configuración de permisos de usuario siguiendo los pasos que se indican a continuación en <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>Confirme si el administrador del sistema de la organización de Adobe le ha otorgado una función de administrador de productos de Adobe. Contacto <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe del Servicio de atención al cliente</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> para averiguar quién en su organización tiene privilegios de administrador en la consola. <br>Aceptar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">la invitación "Administrador de productos de Dynamic Chat"</a>. El <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">correo electrónico de bienvenida</a> se envía cuando Dynamic Chat está habilitado en la instancia de Marketo Engage y usted ha sido designado como administrador del sistema.  <br>Asigne todos los usuarios adecuados al perfil de producto del Marketo Engage en Adobe Admin Console. <br>No puede asignar los roles de los usuarios en Marketo Engage/Administrador/Usuarios y roles antes de agregarlos a un perfil de producto.  <br>Si se agrega un usuario no deseado a varios perfiles de producto, debe eliminar el usuario de todos los perfiles de producto. De lo contrario, seguirán teniendo acceso a Dynamic Chat. </td>
    <td> </td>
  </tr>
  <tr>
    <td>Punto de inicio (si corresponde) </td>
    <td>Configure los que sean necesarios <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> servicios para su empresa.  <br>NOTA: Los seminarios web interactivos son una función integrada de seminarios web con integración nativa con Adobe Connect. No se necesita ninguna integración adicional, pero su instancia deberá hacer lo siguiente <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">sincronizar con Adobe Connect as a LaunchPoint Service.</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">Integraciones adicionales</a> </td>
  </tr>
  <tr>
    <td>Webhooks (si procede)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Cree los Webhooks necesarios</a> para su negocio.  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">Crear un webhook</a> </td>
  </tr>
</tbody>
</table>

## Cofre del tesoro {#treasure-chest}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elemento de acción</th>
    <th>Prioridad</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Cofre del tesoro</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Habilitar el cofre del tesoro</a> para experimentar con características de pilotaje.  <br>Determine las funciones que desea activar o desactivar.</td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Inspector de campaña </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Activar el Inspector de campaña</a> para ver todas las campañas inteligentes a la vez.</td>
    <td>Texto</td>
  </tr>
</tbody>
</table>
