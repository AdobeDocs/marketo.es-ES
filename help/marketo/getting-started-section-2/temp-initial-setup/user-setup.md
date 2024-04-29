---
description: 'Lista de comprobación de configuración anticipada: documentos de Marketo, documentación del producto'
title: Lista de comprobación de configuración anticipada
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# NUEVA ÁREA: Lista de comprobación de configuración anticipada {#early-setup-checklist}

Texto de introducción.

## Marketo Engage en Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrador de productos de Marketo Engage y suscripción </td>
    <td><li>Confirme que el administrador del sistema de su organización de Adobe le ha otorgado una función de administrador de productos de Adobe.</li>  
    <ul>
    <li>Contacto <a href="https://helpx.adobe.com/contact.html">Adobe del Servicio de atención al cliente</a> para averiguar quién de los miembros de su organización ha <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Administrador del sistema de Adobe Admin Console</a> privilegios.</li></ul>
    <li>Acepte la invitación "Marketo Engage Product Admin" para activar su Adobe ID. El <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">correo electrónico de bienvenida</a> se envía cuando se asigna la función en Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Perfiles de producto</td>
    <td><li>Asignar todos los usuarios adecuados al Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Perfil del producto</a> en Adobe Admin Console.</li>
    <ul>
    <li>No puede asignar los roles de los usuarios en Marketo Engage/Administrador/Usuarios y roles antes de agregarlos a un perfil de producto.</li>
    <li>Cada suscripción será un perfil de producto independiente. Si se agrega un usuario no deseado a varios perfiles de producto (por ejemplo, producción y prueba de zona protegida), debe eliminar el usuario de todos los perfiles de producto. De lo contrario, seguirán teniendo acceso a Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Usuarios</td>
    <td><li>Crear una directiva sobre cuándo <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">crear un usuario</a>.</li> <li>Cree una directiva sobre cuándo quitar usuarios.</li>
    <li>Determine quién debe tener <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Permisos de administrador del sistema de Adobe y administrador de productos de Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Adición de usuarios</a> al Perfil de producto deseado.</li>
    <li>Cree un usuario de API para cada caso de uso de API.</li></td>
  </tr>
  <tr>
    <td>Administrador de soporte de productos </td>
    <td><li>Hasta <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">enviar un ticket de asistencia en Adobe Admin Console</a>Además, necesita que un administrador del sistema asigne la función "Administrador de asistencia técnica del producto" a las suscripciones que administra. Solamente un administrador del sistema de su organización puede <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">asignarle a esta función</a>.</li>
    <li>Es posible que el administrador del sistema le haya enviado un correo electrónico en el que se indica que usted es el administrador de asistencia técnica de su suscripción de Marketo Engage. Si es así, haga clic en <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">"Introducción" en el correo electrónico</a> para unirse a la organización.</li>
    <li>Determine los contactos adecuados (con al menos un contacto de copia de seguridad) y pida al administrador del sistema que asigne la función de administrador de soporte técnico del producto por adelantado.</li></td>
  </tr>
</tbody>
</table>

## Configuración del Dynamic Chat en Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

TEXTO

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrador de productos de Dynamic Chat y suscripción (si corresponde) </td>
    <td><li>Confirme si el administrador del sistema de la organización de Adobe le ha otorgado una función de administrador de productos de Adobe. Contacto <a href="https://helpx.adobe.com/contact.html">Adobe del Servicio de atención al cliente</a> para averiguar quién en su organización tiene privilegios de administrador en la consola.</li>
    <li>Aceptar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">la invitación "Administrador de productos de Dynamic Chat"</a>. El <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">correo electrónico de bienvenida</a> se envía cuando Dynamic Chat está habilitado en la instancia de Marketo Engage y usted ha sido designado como administrador del sistema.</li></td>
  </tr>
  <tr>
    <td>Perfiles de producto </td>
    <td><li>Asigne todos los usuarios adecuados al perfil de producto del Dynamic Chat en Adobe Admin Console.</li> 
    <ul>
    <li>Si se añade un usuario no deseado a varios perfiles de producto, debe eliminar el usuario de todos los perfiles de producto. De lo contrario, seguirán teniendo acceso a Dynamic Chat.</li>
    <li>Puede <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">editar perfiles de producto en Dynamic Chat</a> y crear un perfil personalizado con un conjunto personalizado de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">permisos disponibles en su suscripción</a>.</li></td>
  </tr>
  <tr>
    <td>Usuarios </td>
    <td><li>Crear una directiva sobre cuándo agregar y quitar un usuario de chat.</li>
    <li>Cree una política sobre quién debería tener <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat Permisos de administración de productos.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Añada usuarios al perfil de producto deseado</a>.</li></td>
  </tr>
</tbody>
</table>

## Configurar comunicaciones y actualizaciones continuas del sistema

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe Actualizaciones de estado de Marketo </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Suscribirse a las actualizaciones de estado de Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notificaciones </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Suscribirse a las notificaciones de administración</a> para problemas críticos, como errores en las campañas inteligentes y problemas críticos encontrados con la sincronización de CRM.</li></td>
  </tr>
</tbody>
</table>
