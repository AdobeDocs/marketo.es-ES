---
description: Antes de sumergirse en la nueva instancia de Marketo Engage, deberá completar algunos pasos básicos para un uso continuo. Estos pasos incluyen la configuración de la cuenta de usuario, la configuración de administración de soporte y la suscripción a actualizaciones continuas del sistema.
short-description: Después de completar los pasos de configuración iniciales, aprenda a establecer elementos básicos para garantizar un uso continuo y sin problemas.
title: Lista de comprobación de configuración de usuario
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 384740fdfc1f6950369116bd77ee49f9e745bdf1
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Lista de comprobación de configuración de usuario {#user-setup-checklist}

Ahora que ha completado todos los [pasos iniciales de configuración](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}, es hora de establecer algunos elementos básicos para garantizar un uso continuo y sin problemas. Esto sentará las bases para su recorrido con Marketo Engage y le ayudará a aprovechar al máximo sus características. ¡Vamos a empezar!

>[!NOTE]
>
>También puede descargar esta lista de comprobación, [junto con una lista de prácticas recomendadas](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) para su nueva instancia y comprobar los pasos a medida que avanza.

## Marketo Engage en Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Las nuevas suscripciones de Marketo Engage se han incorporado a [Adobe Identity Management System (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). Continúe con la siguiente revisión de la administración de usuarios en Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrador de productos de Marketo Engage y suscripción</td>
    <td><li>Confirme que el administrador del sistema de su organización de Adobe le ha otorgado una función de administrador de productos de Adobe.</li> 
    <ul>
    <li>Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) o envíe un correo electrónico a <code>marketocares@marketo.com</code> para averiguar quién en su organización tiene privilegios de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Administrador del sistema de Adobe Admin Console</a>.</li></ul>
    <li>Acepte la invitación "Marketo Engage Product Admin" para activar su Adobe ID. El <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">correo electrónico de bienvenida</a> se envía cuando se asigna la función en Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Perfiles de producto</td>
    <td><li>Asigne todos los usuarios deseados al Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Perfil del producto</a> en Adobe Admin Console.</li>
    <ul>
    <li>No puede asignar los roles de los usuarios en Marketo Engage &gt; Administración &gt; Usuarios y roles antes de añadirlos a un perfil de producto.</li>
    <li>Cada suscripción será un perfil de producto independiente. Si se agrega un usuario no deseado a varios perfiles de producto (por ejemplo, producción y prueba de zona protegida), debe eliminar el usuario de todos los perfiles de producto. De lo contrario, seguirán teniendo acceso a Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Usuarios</td>
    <td><li>Crear una directiva sobre cuándo <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">crear un usuario</a>.</li> <li>Cree una directiva sobre cuándo quitar usuarios.</li>
    <li>Determine quién debe tener <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">permisos de administrador de sistemas de Adobe y administrador de productos de Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Agregar usuarios</a> al perfil de producto deseado.</li>
    <li>Cree un usuario de API para cada caso de uso de API.</li></td>
  </tr>
  <tr>
    <td>API de administración de usuarios (si corresponde)</td>
    <td><li>Use la <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">API de administración de usuarios de Adobe</a> para invitar, actualizar y eliminar usuarios.</li>
    <li>Use la <a href="https://developer.adobe.com/umapi/">API de administración de usuarios de Adobe</a> para agregar o quitar roles (por ejemplo, administradores, administradores de soporte, desarrolladores).</li>
    </td>
  </tr>
  <tr>
    <td>Administrador de soporte de productos</td>
    <td><li>Para <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">enviar un ticket de soporte en Adobe Admin Console</a>, necesita que un administrador del sistema asigne la función 'Administrador de soporte de producto' a las suscripciones que administra. Solo un administrador del sistema de su organización puede <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">asignarle a usted este rol</a>.</li>
    <li>Es posible que el administrador del sistema le haya enviado un correo electrónico en el que se indica que usted es el administrador de asistencia técnica de su suscripción de Marketo Engage. Si es así, haga clic en <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">'Comenzar'</a> en el correo electrónico para unirse a la organización.</li>
    <li>Determine los contactos adecuados (con al menos un contacto de copia de seguridad) y pida al administrador del sistema que asigne la función de administrador de soporte técnico del producto.</li></td>
  </tr>
</tbody>
</table>

## Configuración del Dynamic Chat en Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Para usar [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html), el canal nativo de automatización de conversaciones en Marketo Engage, continúa con la configuración de permisos de usuario siguiendo los pasos que se indican a continuación en [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}.

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrador de productos de Dynamic Chat y suscripción (si corresponde)</td>
    <td><li>Confirme que el administrador del sistema de su organización de Adobe le ha otorgado una función de administrador de productos de Adobe.</li> 
    <ul><li>Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) o envíe un correo electrónico a <code>marketocares@marketo.com</code> para averiguar quién en su organización tiene privilegios de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Administrador del sistema de Adobe Admin Console</a>.</li></ul>
    <li>Acepte la invitación de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">'Administrador de productos de Dynamic Chat'</a>. El <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">correo electrónico de bienvenida</a> se envía cuando el Dynamic Chat está habilitado en la instancia de Marketo Engage y usted ha sido designado como administrador del sistema.</li></td>
  </tr>
  <tr>
    <td>Perfiles de producto</td>
    <td><li>Asigne todos los usuarios deseados al perfil de producto del Dynamic Chat en Adobe Admin Console.</li> 
    <ul>
    <li>Si se añade un usuario no deseado a varios perfiles de producto, debe eliminar el usuario de todos los perfiles de producto. De lo contrario, seguirán teniendo acceso a Dynamic Chat.</li>
    <li>Puede <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">editar perfiles de producto en Dynamic Chat</a> y crear un perfil personalizado con un conjunto personalizado de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">permisos disponibles en su suscripción</a>.</li></td>
  </tr>
  <tr>
    <td>Usuarios</td>
    <td><li>Crear una directiva sobre cuándo agregar y quitar un usuario de chat.</li>
    <li>Cree una directiva sobre quién debe tener <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">permisos de administrador de productos de Adobe Dynamic Chat.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Agregar usuarios al perfil de producto deseado</a>.</li></td>
  </tr>
</tbody>
</table>

## Configurar comunicaciones y actualizaciones continuas del sistema {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe Actualizaciones de estado de Marketo</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Suscribirse a las actualizaciones de estado de Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notificaciones</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Suscríbase a las notificaciones de administración</a> para problemas críticos como errores en sus campañas inteligentes y problemas críticos encontrados con la sincronización de CRM.</li></td>
  </tr>
</tbody>
</table>

<p>

Ahora que su cuenta de Marketo Engage está lista, revise nuestra sección [Prácticas recomendadas para una nueva instancia de Marketo Engage](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} para aprovechar al máximo su inversión y prepararse para tener éxito a largo plazo.
