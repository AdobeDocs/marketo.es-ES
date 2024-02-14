---
description: 'NUEVA ÁREA: Documentos de Marketo: documentación del producto'
title: NUEVA ÁREA
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: a1c06c980a6f8955f4f51e2fc85202d77a8f27da
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 4%

---

# NUEVA ÁREA: Lista de comprobación de administración {#new-area-admin-checklist}

Abriendo propaganda

## Funciones {#roles}

<table>
<thead>
  <tr>
    <th>Área </th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Funciones </td>
    <td><li>Revise las funciones prediseñadas y confirme qué permisos/acceso tiene cada función.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Crear una función nueva</a> o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">editar los roles</a> en función de las necesidades de su organización y de la frecuencia con la que los usuarios inicien sesión.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Asignar usuarios a las funciones adecuadas</a>.</li>
    <li>Después de asignar las funciones de los usuarios, revise el número de usuarios por función.</li>  <li>Implemente una función única para cada usuario de API para facilitar la resolución de problemas.</li></td>
  </tr>
  <tr>
    <td>Documentación </td>
    <td>Defina usuarios y funciones para su organización. <br>Defina el proceso para agregar un nuevo usuario/administrador. </td>
  </tr>
  <tr>
    <td>Zona protegida (si corresponde) </td>
    <td>Revise las categorías anteriores para su zona protegida si tiene una. </td>
  </tr>
</tbody>
</table>

## Espacios de trabajo y particiones {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espacios de trabajo y particiones </td>
    <td><li>Determinar el número de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> workspaces</a> y/o particiones que su organización necesita tener y <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">cuántos usuarios tienen acceso a cada espacio de trabajo.</a></li>
    <li>Defina el propósito principal de cada espacio de trabajo y partición.</li>
    <li>Definir la relación entre los espacios de trabajo y las particiones.</li></td>
  </tr>
  <tr>
    <td>Documentación </td>
    <td><li>Documente cómo se definen los espacios de trabajo y cómo se relacionan con las particiones de la base de datos (es decir, un espacio de trabajo global que vea a todos, en comparación con los sectores empresariales).</li>
    <li>Importe los registros nuevos a la partición apropiada.</li>
    <li>Defina el valor en CRM que coloca a los usuarios en la partición apropiada.</li></td>
  </tr>
</tbody>
</table>

## Configuración de campañas inteligentes {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Configuración de campañas inteligentes </td>
    <td><li>Añadir un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">restricción en el tamaño de la campaña inteligente</a>, evitando el envío accidental de toda la base de datos.</li>
    <li>Habilitar restricciones de persona para campañas inteligentes</li></td>
  </tr>
</tbody>
</table>

## Configuración del correo electrónico {#email-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Valores predeterminados de correo electrónico</td>
    <td><li>En Dominio de marca, seleccione su dominio y añada su CNAME de correo electrónico. Debe tener el siguiente formato: [EmailTrackingCNAME].[CompanyDomain].com.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Configuración de SPF y DKIM</a> para la entrega de correo electrónico.</li></td>
  </tr>
</tbody>
</table>

## Límites de comunicación {#communication-limits}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Límites de comunicación</td>
    <td><li>Lugar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Límites de comunicación</a>.</li>
    <li>Determine si su empresa requiere una política sobre límites de comunicación.</li></td>
  </tr>
</tbody>
</table>

## Etiquetas {#tags}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canales</td>
    <td><li>Defina cómo utilizar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">canales</a>.</li></td>
  </tr>
  <tr>
    <td>Etiquetas </td>
    <td><li>Defina cómo utilizar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">etiquetas</a>.</li></td>
  </tr>
  <tr>
    <td>Calendario (si procede) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Puestos del calendario de marketing de problemas</a> para aquellos que necesitan acceso.</li> 
    <li>Configuración de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Calendario</a>.</li></td>
  </tr>
</tbody>
</table>

## Administración de bases de datos {#database-management}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administración de campos</td>
    <td><li>Implementar la convención de nombres para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">campos personalizados.</a> Por ejemplo, comience por "MKTO".</li>
    <li>Sea selectivo sobre los campos que sincroniza. Cuantos más campos sincronice, más lento será el ciclo de sincronización.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Bloquear actualizaciones de campos</a> desea que se escriba una vez (es decir, origen del posible cliente original, detalle del origen del posible cliente original, campos de UTM de primer contacto, etc.).</li></td>
  </tr>
  <tr>
    <td>Actividades personalizadas </td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">Actividades personalizadas</a> que son específicos de su negocio.</li></td>
  </tr>
  <tr>
    <td>Objetos personalizados </td>
    <td><li>Revisar cuántos <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">Objetos personalizados</a> lo necesitas.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">Sincronizar esos objetos personalizados con su CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## Integraciones {#integrations}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Iniciar sincronización de CRM. Elija entre las siguientes opciones, según el CRM que utilice su compañía: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>Identifique el tipo de acceso que necesita para acceder a su CRM.</li>
    <li>Identifique al administrador de CRM para la resolución de problemas.</li></td>
  </tr>
  <tr>
    <td>Perspectiva de ventas (si corresponde)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">Configurar perspectiva de ventas.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">Emita puestos para los usuarios adecuados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">Configuración de la API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">Personalizar las puntuaciones de los posibles clientes.</a></li></td>
  </tr>
</tbody>
</table>
