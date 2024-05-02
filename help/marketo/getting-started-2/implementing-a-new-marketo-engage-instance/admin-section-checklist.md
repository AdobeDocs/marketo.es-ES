---
description: Configure la sección Admin para la nueva instancia de Marketo Engage.
title: 'Nuevas prácticas recomendadas para instancias: lista de comprobación de la sección de administración'
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: fa5b686aabd3aab2d9020758fde00ed06564c76c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 6%

---

# Prácticas recomendadas para nuevas instancias: Lista de comprobación de sección de administración {#new-instance-best-practices-admin-section-checklist}

Como administrador nuevo que navega por una nueva instancia de Marketo Engage, aplique la lista de comprobación siguiente para guiarle a través del proceso de implementación. Al igual que con todas estas guías, puede descargar las listas de comprobación [VÍNCULO] y realice un seguimiento de su progreso.

## Roles {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Roles</td>
    <td><li>Revise las funciones prediseñadas y confirme qué permisos/acceso tiene cada función.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Crear una función nueva</a> o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">editar los roles</a> en función de las necesidades de su organización.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Asignar usuarios a las funciones adecuadas</a>. Los usuarios deben añadirse a la suscripción en Adobe Admin Console antes de conceder sus funciones en Funciones. Consulte la sección "Usuarios" en la <a href="/help/marketo/getting-started-2/initial-setup/user-setup.md">Lista de comprobación de configuración inicial</a>.</li>
    <li>Después de asignar las funciones de los usuarios, revise el número de usuarios por función.</li>
    <li>Implemente una función única para cada usuario de API para facilitar la resolución de problemas.</li></td>
  </tr>
  <tr>
    <td>Documentación</td>
    <td><li>Defina usuarios y funciones para su organización.</li>
    <li>Defina el proceso para agregar un nuevo usuario/administrador.</li></td>
  </tr>
  <tr>
    <td>Zona protegida (si corresponde)</td>
    <td><li>Revise las categorías anteriores para su <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md">espacio aislado</a>.</li></td>
  </tr>
</tbody>
</table>

## Esp. de trab. y particiones {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espacios de trabajo y particiones (si corresponde)</td>
    <td><li>Determinar el número de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> workspaces</a> y/o particiones que su organización necesita tener y <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">cuántos usuarios tienen acceso a cada espacio de trabajo.</a></li>
    <li>Defina el propósito principal de cada espacio de trabajo y partición.</li>
    <li>Definir la relación entre los espacios de trabajo y las particiones.</li></td>
  </tr>
  <tr>
    <td>Documentación</td>
    <td><li>Documente cómo se definen los espacios de trabajo y cómo se relaciona con las particiones de la base de datos (por ejemplo, un espacio de trabajo global que muestre todos los usuarios frente a los sectores empresariales).</li>
    <li>Importe nuevos registros a la partición apropiada.</li>
    <li>Defina el valor en su CRM que coloca a los usuarios en la partición apropiada.</li></td>
  </tr>
</tbody>
</table>

## Configuración de la campaña inteligente {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Configuración de la campaña inteligente</td>
    <td><li>Añadir un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">restricción en el tamaño de la campaña inteligente</a>, evitando enviar por correo electrónico accidentalmente toda la base de datos.</li></td>
  </tr>
</tbody>
</table>

## Configuración del email {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Valores predeterminados de correo electrónico</td>
    <td><li>En Dominio de marca, seleccione su dominio y añada su CNAME de correo electrónico. Debe tener el siguiente formato: [EmailTrackingCNAME].[CompanyDomain].com.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Póngase en contacto con Soporte técnico de Marketo</a> para protegerlo con una provisión de certificado SSL. Este proceso puede tardar hasta tres días hábiles en completarse.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Configuración de SPF y DKIM</a> para la entrega de correo electrónico.</li></td>
  </tr>
</tbody>
</table>

## Límites de comunicación {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Límites de comunicación</td>
    <td><li>Iniciar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">límites de comunicación</a>.</li>
    <li>Determine si su empresa requiere una política sobre límites de comunicación.</li></td>
  </tr>
</tbody>
</table>

## Etiquetas {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canales</td>
    <td><li>Defina cómo utilizar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">canales</a>.</li></td>
  </tr>
  <tr>
    <td>Etiquetas</td>
    <td><li>Defina cómo utilizar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">etiquetas</a>.</li></td>
  </tr>
  <tr>
    <td>Calendario (si procede)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">Puestos del calendario de marketing de problemas</a> para aquellos que necesitan acceso.</li>
    <li>Configure las variables <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">Calendario</a>.</li></td>
  </tr>
</tbody>
</table>

## Administración de bases de datos {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administración de campos</td>
    <td><li>Implementación de una convención de nombres para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">campos personalizados</a> (por ejemplo, comenzando con "MKTO").</li>
    <li>Sea selectivo sobre los campos que sincroniza. Cuantos más campos sincronice, más lento será el ciclo de sincronización.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Bloquear actualizaciones de campos</a> desea que se escriba una vez (por ejemplo, origen del posible cliente original, detalles del origen del posible cliente original, campos de UTM de primer contacto, etc.).</li></td>
  </tr>
  <tr>
    <td>Actividades personalizadas</td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Actividades personalizadas</a> que son específicos de su negocio.</li></td>
  </tr>
  <tr>
    <td>Objetos personalizados</td>
    <td><li>Revisar cuántos <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Objetos personalizados</a> lo necesitas.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Sincronizar esos objetos personalizados con su CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## Integraciones {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>Iniciar sincronización de CRM. Elija entre las siguientes opciones, según el CRM que utilice su compañía: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>.</li>
    <li>Identifique el tipo de acceso que necesita para acceder a su CRM.</li>
    <li>Identifique al administrador de CRM para la resolución de problemas.</li></td>
  </tr>
  <tr>
    <td>Servicios web</td>
    <td><li>Determine los usuarios/aplicaciones que pueden hacer lo siguiente <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">Llamadas de API</a> en su instancia.</li>
    <li>Revise todas las aplicaciones que realizarán llamadas de API y determine si es necesario un aumento o una disminución de las llamadas de API.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configuración de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> servicios para su empresa. Cada LaunchPoint debe estar emparejado con un usuario único de la API para ayudar a solucionar problemas.</li></td>
  </tr>
  <tr>
    <td>Seminarios web interactivos (si corresponde)</td>
    <td>NOTA: Los seminarios web interactivos solo se proporcionan a instancias de producción.
    <li>Para crear seminarios web interactivos, la función de seminarios web integrada, <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">añadir usuarios a la sección "Usuario"</a> en la pestaña Seminario web interactivo.</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (si procede)</td>
    <td><li>Asignar usuarios a <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Funciones de "Dynamic Chat de acceso"</a> en Marketo Engage &gt; Administración &gt; Usuarios y funciones.</li></td>
  </tr>
  <tr>
    <td>Perspectiva de ventas (si corresponde)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Configurar la acción de información de ventas</a> en Perspectiva de ventas &gt; Configuración de acciones.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Emitir puestos para los usuarios adecuados</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">Configuración de la API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Personalizar las puntuaciones de los posibles clientes</a>.</li></td>
  </tr>
  <tr>
    <td>Conexión de ventas (si corresponde)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Invite a los administradores de Marketo Engage correspondientes a la instancia de Sales Connect</a>.</li>
    <li>Complete la <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">configuración de administración de Sales Connect adicional</a> en Sales Connect y Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (si procede)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html">Cree los Webhooks necesarios</a> para su negocio.</li>
    </td>
  </tr>
</tbody>
</table>

## Cofre del tesoro {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Cofre del tesoro </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Habilitar el cofre del tesoro</a> para experimentar con características de pilotaje.</li>
    <li>Determine las funciones que desea activar o desactivar.</li></td>
  </tr>
  <tr>
    <td>Inspector de campañas </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Activar el Inspector de campaña</a> para ver todas las campañas inteligentes a la vez.</li></td>
  </tr>
</tbody>
</table>
