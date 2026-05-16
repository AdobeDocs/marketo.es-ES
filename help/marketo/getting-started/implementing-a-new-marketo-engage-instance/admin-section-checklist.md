---
description: Configure la sección Administración para la nueva instancia de Marketo Engage.
title: 'Nuevas prácticas recomendadas para instancias: lista de comprobación de la sección de administración'
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
TQID: https://experienceleague.adobe.com/9yNDZl4AGlgdf3FRLib3H7wVhKYTciLSXevJ0JTEFjQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
subfeature_v2:
  - id: a572083b-9238-40c5-8a10-cf294c415aab
  - id: a8c137b3-8aa5-433e-bdc9-0a216c2a11c1
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
  - id: cbccec41-b38b-4693-8acf-fed684dd06ba
  - id: de9e3aa9-f002-4fe1-897b-09ee3c55114b
  - id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
  - id: f5e85a9b-a883-40d0-8759-f3651efb32e9
  - id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 1125
ht-degree: 4%

---

# Prácticas recomendadas para nuevas instancias: Lista de comprobación de sección de administración {#new-instance-best-practices-admin-section-checklist}

Como administrador nuevo que navega por una nueva instancia de Marketo Engage, aplique la lista de comprobación siguiente para guiarle a través del proceso de implementación. Al igual que con todas estas guías, también puede [descargar las listas de comprobación](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) y realizar un seguimiento de su progreso.

## Funciones {#roles}

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
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=es#create-a-new-role" target="_blank">Cree una nueva función</a> o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=es#edit-a-role" target="_blank">edite las funciones</a> según las necesidades de su organización.</li>
    <li><a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Asigne usuarios a los roles correspondientes</a>. Los usuarios deben añadirse a la suscripción en Adobe Admin Console antes de conceder sus funciones en "Funciones". Consulte la sección Usuarios en la <a href="/help/marketo/getting-started/initial-setup/user-setup.md">lista de comprobación de la configuración inicial</a>.</li>
    <li>Después de asignar las funciones de los usuarios, revise el número de usuarios por función.</li>
    <li>Implemente una función única para cada usuario de API para facilitar la resolución de problemas.</li></td>
  </tr>
  <tr>
    <td>Zona protegida (si corresponde)</td>
    <td><li>Revise las categorías anteriores para su <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">zona protegida</a>.</li></td>
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
    <td><li>Determine el número de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=es" target="_blank"> espacios de trabajo</a> y/o particiones que su organización necesita tener, y <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=es" target="_blank">cuántos usuarios tienen acceso a cada espacio de trabajo.</a></li>
    <li>Defina el propósito principal de cada espacio de trabajo y partición.</li>
    <li>Definir la relación entre los espacios de trabajo y las particiones.</li></td>
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
    <td><li>Agregue una restricción <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=es" target="_blank">en el tamaño de la campaña inteligente</a>, para evitar enviar por correo electrónico accidentalmente toda la base de datos.</li></td>
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
    <td><li>Implementar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=es" target="_blank">límites de comunicación</a>.</li>
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
    <td><li>Defina cómo usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=es" target="_blank">canales</a>.</li></td>
  </tr>
  <tr>
    <td>Etiquetas</td>
    <td><li>Defina cómo usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=es" target="_blank">etiquetas</a>.</li></td>
  </tr>
  <tr>
    <td>Calendario<br>
    (si procede)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=es" target="_blank">Asientos del calendario de mercadotecnia de problemas</a> para quienes necesitan acceso.</li>
    <li>Configurar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=es" target="_blank">Calendario</a>.</li></td>
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
    <td><li>Implemente una convención de nombres para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=es" target="_blank">campos personalizados</a> (por ejemplo, a partir de "MKTO").</li>
    <li>Sea selectivo sobre los campos que sincroniza. Cuantos más campos sincronice, más lento será el ciclo de sincronización.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=es" target="_blank">Bloquear las actualizaciones de los campos</a> en los que desee que se escriban una sola vez (por ejemplo, origen del posible cliente original, detalles del origen del posible cliente original, campos de UTM de primer contacto, etc.).</li></td>
  </tr>
  <tr>
    <td>Actividades personalizadas</td>
    <td><li>Defina <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=es" target="_blank">actividades personalizadas</a> que sean específicas de su negocio.</li></td>
  </tr>
  <tr>
    <td>Objetos personalizados</td>
    <td><li>Revise cuántos <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=es" target="_blank">objetos personalizados</a> necesita.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=es" target="_blank">Sincroniza esos objetos personalizados</a> con tu CRM.</li></td>
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
    <td><li>Identifique los permisos que necesita para acceder a su CRM.</li>
    <li>Identifique al administrador de CRM para la resolución de problemas.</li></td>
  </tr>
  <tr>
    <td>Servicios web</td>
    <td><li>Determine los usuarios/aplicaciones que pueden hacer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=es" target="_blank">llamadas a la API</a> en su instancia.</li>
    <li>Revise todas las aplicaciones que realizarán llamadas de API y determine si es necesario un aumento o una disminución de las llamadas de API.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configure los servicios de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=es" target="_blank">LaunchPoint</a> para su empresa. Cada LaunchPoint debe estar emparejado con un usuario único de la API para ayudar a solucionar problemas.</li></td>
  </tr>
  <tr>
    <td>Seminarios web interactivos (si corresponde)</td>
    <td><li>Para crear seminarios web interactivos, la característica de seminarios web integrados de Marketo Engage, <a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">agregue usuarios a la sección 'Usuario'</a> de la ficha Seminario web interactivo.</li>
    <p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Los seminarios web interactivos solo se proporcionan a instancias de producción.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (si corresponde)</td>
    <td><li>Asigne usuarios a <a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">'Acceder a los roles de Dynamic Chat'</a> en Marketo Engage &gt; Administración &gt; Usuarios y roles.</li></td>
  </tr>
  <tr>
    <td>Insight de ventas (si corresponde)</td>
    <td><li><a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Configurar la acción de Insight de ventas</a> en Sales Insight &gt; Configuración de acciones.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=es#invite-individual-users-to-msi-actions" target="_blank">Puestos del problema</a> a los usuarios correspondientes.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=es" target="_blank">Configurar la API</a>.</li>
    <li>Personalizar las <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=es" target="_blank">puntuaciones de posibles clientes</a>.</li></td>
  </tr>
  <tr>
    <td>Conexión de ventas (si corresponde)</td>
    <td><li>Invite a los administradores de Marketo Engage correspondientes a la <a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">instancia de Sales Connect</a>.</li>
    <li>Complete la <a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">configuración adicional del administrador de Sales Connect</a> en Sales Connect y Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (si procede)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=es" target="_blank">Cree los Webhooks necesarios</a> para su empresa.</li>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=es" target="_blank">Habilitar Treasure Chest</a> para experimentar con características de prueba.</li>
    <li>Determine las funciones que desea activar o desactivar.</li></td>
  </tr>
  <tr>
    <td>Inspector de campañas </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=es" target="_blank">Activa el Inspector de campañas</a> para ver todas tus campañas inteligentes en un solo lugar.</li></td>
  </tr>
</tbody>
</table>
