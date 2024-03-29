---
description: Lista de comprobación de administración de instancias heredadas - Documentos de Marketo - Documentación del producto
title: Lista de comprobación de administración de instancias heredadas
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: 0ca63c52cb255cc41cbb53b2c481e589d08004b3
workflow-type: tm+mt
source-wordcount: '1846'
ht-degree: 1%

---

# Instancia heredada: Lista de comprobación de sección de administración {#inherited-instance-admin-section-checklist}

Las listas de comprobación siguientes (listas de comprobación subsiguientes vinculadas al final de cada artículo) han sido elaboradas por Adobe Professional Services con los datos de Marketo Champions para ayudarle a ponerse al día rápidamente. También puede [descargar las listas de comprobación](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) y realice un seguimiento de su progreso.

>[!TIP]
>
>Si es un usuario Marketo Engage nuevo y no está familiarizado con muchos de los términos, consulte la [Glosario del Marketo Engage](/help/marketo/getting-started/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Esto solo es aplicable a las suscripciones de Marketo Engage incorporadas a [Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. If your subscription has not onboarded Adobe IMS yet, proceed with the [legacy user roles and permissions experience](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} en Marketo Engage > Administración > Usuarios y funciones.

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th> 
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Administrador de productos de Marketo Engage y suscripción</td> 
   <td><li>¿Se ha migrado su suscripción de Marketo Engage a <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> ¿todavía? 
<br/>     Si es así, ¿su "administrador del sistema de Adobe Admin Console" le ha concedido una función "Administrador de productos de Adobe Admin Console"? Si no está seguro de qué persona de su organización tiene privilegios de administrador en la consola, póngase en contacto con <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe del Servicio de atención al cliente</a>.</li>
<li>¿Ha aceptado la invitación de "Marketo Engage Product Admin"? El correo electrónico se envía cuando se asigna la función en Adobe Admin Console.
<br/>     Si no es así, busque el <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">correo electrónico de bienvenida</a> en la bandeja de entrada y acepte la invitación para activar el Adobe ID.</li></td>
  </tr>
  <tr> 
   <td>Perfil del producto</td> 
   <td><li>¿Están asignados todos los usuarios adecuados al perfil de producto del Marketo Engage en Adobe Admin Console?
<br/>     Si no es así, asegúrese de <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">agregar o quitar usuarios</a> de perfiles de producto del Marketo Engage en Adobe Admin Console. No se pueden asignar funciones de usuario en Marketo Engage &gt; Administración &gt; Usuarios y funciones si se añaden a un perfil de producto.</li>
<p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Si se añade un usuario no deseado a varios perfiles de producto, debe eliminar el usuario de todos los perfiles de producto. De lo contrario, seguirán teniendo acceso a Marketo Engage.</td>
  </tr>
  <tr> 
   <td>API de administración de usuarios</td> 
   <td><li>¿Su suscripción utiliza alguna API de administración de usuarios de Marketo?
<br/>     Si es así, deberá utilizar <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">API de IMS de Adobe</a> para invitar, actualizar y eliminar usuarios a partir de ahora.</li>
<p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: "Administración de funciones" permanece en Marketo Engage y las API de administración de usuarios de Marketo se pueden seguir utilizando para la administración de funciones.</td>
  </tr>
 </tbody> 
</table>

## Usuarios y funciones {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Usuarios</td> 
   <td><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Si su suscripción ya está en Adobe IMS, continúe con la siguiente revisión de la administración de usuarios en Adobe Admin Console. De lo contrario, vaya a Administración &gt; Usuarios y funciones &gt; Usuarios en Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Cuántos usuarios</a> ¿hay?</li>
<li>¿Hay algún usuario que debería ser <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">eliminado</a>?</li>
<li>¿Su compañía tiene directivas para eliminar usuarios?</li> 
<li>Cuántos usuarios tienen <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Permisos de administración</a>?</li>
<li>Si alguno de estos usuarios se cambia a <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">¿otros roles?</a></li> 
<li>¿Quiénes son los <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">Usuarios de API</a> en este caso?</li></td>
  </tr>
  <tr> 
   <td>Funciones</td> 
   <td><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Tanto si utiliza Marketo con identidad de Adobe como si no, revise los permisos de funciones en Marketo Engage en Administración &gt; Usuarios y funciones &gt; Funciones.
   <p><li>¿Cuántos roles hay?</li>  
<li>Qué <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permisos/acceso</a> ¿tiene cada función? ¿Se debe realizar algún ajuste?</li>
<li>¿Cuántos usuarios hay por función?</li>
<li>La frecuencia con la que los usuarios <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">iniciar sesión</a>?</li>
<li>¿Cada usuario de API tiene su <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">función de usuario propio</a>? Si no es así, considere implementar esto para facilitar la resolución de problemas.</li> 
<li>¿Se alinean las funciones de usuario y los permisos con las políticas de privacidad de datos corporativas para el cumplimiento de la regulación (por ejemplo, <a href="https://gdpr-info.eu/" target="_blank">RGPD</a>)? Realizar los datos corporativos <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">políticas de privacidad</a> ¿permitir que los usuarios descarguen y compartan datos de usuario del Marketo Engage? ¿Es necesario el negocio de permisos?</li></td>
  </tr>
  <tr> 
   <td>Usuarios de asistencia</td> 
   <td><li>¿Ha configurado el <a href="/help/marketo/getting-started/setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">contactos autorizados</a> en el Portal de asistencia?</li></td>
  </tr>
  <tr> 
   <td>Documentación interna</td> 
   <td><li>¿Los usuarios y las funciones están claramente definidos en su organización?</li>
<li>¿Cuál es su proceso para agregar un nuevo usuario/administrador?</li></td>
  </tr>
  <tr> 
   <td>Zona protegida (si corresponde)</td> 
   <td><li>¿Tiene un <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">instancia de zona protegida</a>?
   <br/>     Si es así, revise las categorías anteriores para su zona protegida.</li>
<li>Es <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Importación de programas</a> ¿está vinculado con su zona protegida?</li></td>
  </tr>
 </tbody> 
</table>

## Pista de auditoría {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Pista de auditoría</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Quién está trabajando</a> en la instancia?</li></td>
  </tr>
 </tbody> 
</table>

## Espacios de trabajo y particiones {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Espacios de trabajo y particiones</td> 
   <td><li>¿Cuántos <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">Espacios de trabajo o particiones</a> ¿tiene usted?</li>
<li>¿Cuál es el propósito principal de cada espacio de trabajo y partición?</li>
<li>Haga lo siguiente <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Workspaces</a> o <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Particiones</a> ¿necesita ser auditado/cambiado?</li>
<li>¿Cuál es la relación entre sus espacios de trabajo y las particiones?</li>
<li>Cuántos usuarios <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">tener acceso</a> a cada Workspace?</li></td>
  </tr>
  <tr> 
   <td>Documentación interna</td> 
   <td><li>¿Cómo se definen los espacios de trabajo y las particiones?</li>
<li>¿Cuál es su proceso para añadir espacios de trabajo a su instancia o añadir usuarios a un espacio de trabajo?</li></td>
  </tr>
 </tbody> 
</table>

## Campañas inteligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Campañas inteligentes</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">¿Tiene una restricción?</a> ¿Cuál es el tamaño de campaña inteligente? 
   <br/>     Si no es así, considere la posibilidad de agregar uno. Se recomienda limitar los límites de Smart Campaign al 25 % de la base de datos para evitar una comunicación excesiva o procesar toda la base de datos en los flujos de trabajo; esto no solo protege la marca, sino que ayuda a proteger el rendimiento de la instancia.</li></td>
  </tr>
 </tbody> 
</table>

## Límites de comunicación {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Límites de comunicación</td> 
   <td><li>¿Hay? <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">límites de comunicación</a> en su lugar? ¿Su empresa tiene políticas en las que podrían ser necesarios límites de comunicación?</li>
<p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Recomendamos limitar su comunicación a 1 por día y a 3 por 7 días, con <b>non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operativo</a> correos electrónicos bloqueados.</td>
  </tr>
 </tbody> 
</table>

## Etiquetas {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Etiquetas</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Cuántas etiquetas</a> ¿hay? ¿Cuántas etiquetas se están utilizando? ¿Es necesario añadir alguna?</li>
<li>¿Se requieren etiquetas dentro de los programas?</li></td>
  </tr>
  <tr> 
   <td>Canales</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Cuántos canales</a> ¿hay? ¿Cuántos están en uso?</li>
<li>Son todos <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">estados de programa de canal adecuados</a>? ¿Muestran progresión dentro del programa?</li>
<li>¿Sus canales están relacionados con tipos de programas específicos?</li>
<li>¿Qué estados se consideran un éxito para cada canal? ¿Se alinean con sus objetivos de marketing?</li>
<li>¿Se está utilizando correctamente el canal operativo?</li>
<li>Para el Report Builder avanzado (Explorador del ciclo de ingresos/RCE), ¿está configurado el comportamiento de análisis de canal para alinearse con las prácticas del programa que incorporan el coste del período?</li></td>
  </tr>
  <tr> 
   <td>Calendario de marketing (si corresponde)</td> 
   <td><li>¿Cuántos <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">tipos de entradas de calendario</a> ¿hay? ¿Siguen siendo relevantes?</li></td>
  </tr>
 </tbody> 
</table>

## Administración de bases de datos {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Administración de campos</td> 
   <td><li>¿Cuántos campos hay? 
   <br/>     Clic <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Exportar nombres de campo</a> para revisar una lista de sus campos, campos personalizados y sus nombres de API.</li>
<li>¿Cuántos <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">campos personalizados</a> ¿hay?</li>
<li>¿Cuántos campos se están utilizando? 
<br/>     Seleccionar <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Exportación utilizada por</a> en la lista desplegable Acciones de campo para revisar los activos relacionados de un campo.</li>
<li>¿Cuántos campos se sincronizan entre Marketo Engage y su CRM?</li>
<li>¿Los campos de CRM están sincronizados con los objetos adecuados?</li>
<li>¿Hay alguna <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">conjunto de vistas personalizadas</a> para obtener detalles de la persona? ¿Debería haber?</li>
<li>¿Tiene una convención de nombres para los campos basada en el origen? 
<br/>     Si no es así, considere implementar esto.</li>
<li>¿Hay algún campo? <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">tapado</a>? 
<br/>     Si es así, asegúrese de comprender por qué lo son.</li></td>
  </tr>
  <tr> 
   <td>Actividades personalizadas</td> 
   <td><li>¿Hay alguna? <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">actividades personalizadas</a>?
<br/>     Si es así, haga clic en ellas para comprender qué actividades no están relacionadas con un formulario, un correo electrónico o una página de aterrizaje de Marketo.</li></td>
  </tr>
  <tr> 
   <td>Objetos personalizados</td> 
   <td><li>¿Cuántos <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">objetos personalizados</a> ¿hay? ¿Cómo se sincronizan con su CRM?</li>
<li>¿Cómo utilizan sus programas y consultas de lista estos objetos personalizados?</li></td>
  </tr>
 </tbody> 
</table>

## Correo electrónico {#email}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Configuración predeterminada de correo electrónico</td> 
   <td><li>En Administración &gt; Correo electrónico, ¿está actualizada la configuración predeterminada (por ejemplo, <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">Correo electrónico/etiqueta "de"</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">dominio de personalización de marca</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">cancelar suscripción de mensaje</a>, etc.)?</li></td>
  </tr>
 </tbody> 
</table>

## Integraciones {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>¿A qué CRM se está sincronizando? ¿Salesforce? ¿MS Dynamics? ¿Veeva?</li>
<li>¿Está utilizando un <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">sincronización personalizada</a>?</li>
<li>[Solo Salesforce] ¿Su instancia tiene implementados los filtros de sincronización personalizados? 
<p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Póngase en contacto con el Soporte técnico de Marketo para identificar los filtros de sincronización personalizados o solicitar que se implemente una regla de sincronización personalizada.</li></td>
  </tr>
  <tr> 
   <td>Páginas de destino</td> 
   <td><li>¿Qué es el <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">dominio establecido como</a>?</li>
   <li>¿Cómo se establece la página principal?</li>
<li>¿Qué es el <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">reserva establecida como</a>?</li>
<li>¿Está habilitado el rellenado previo del formulario?</li>
<li>Son <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">direcciones URL personalizadas</a> ¿habilitado?</li>
<li>¿Hay reglas configuradas para <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">redirecciones</a>?</li>
<li>¿Tiene alias de dominio establecidos? ¿Está realizando un seguimiento de cómo utiliza sus alias de dominio?</li>
<li>Es <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Dominios seguros para páginas de destino</a> ¿habilitado? 
<br/>     Confirme si los recursos de la página de aterrizaje contienen una dirección URL "http".</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Es su <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Código de seguimiento de Munchkin</a> en su sitio web (no una página de aterrizaje de Marketo Engage)?</li>
<li>Es un <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">No rastrear</a> ¿Solicitud de explorador habilitada?</li>
<li>Es su <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">API de Munchkin</a> ¿configurado? 
<p><img src="assets/tip-icon.png" alt="icono de sugerencia">SUGERENCIA: Si falta documentación sobre dónde está el código munchkin en el sitio web, puede ver todas las URL creando un <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Informe de actividad de página web</a>.</li></td>
  </tr>
  <tr> 
   <td>Servicios web</td> 
   <td><li>Son <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">Restricciones de IP</a> ¿habilitado? ¿Deberían estarlo?</li>
<li>¿Qué usuarios/aplicaciones realizan llamadas de API en su instancia?</li>
<li>¿Está alcanzando o cerca de alcanzar su límite de API?
<br/>     Si es así, considere la posibilidad de aumentarla o auditar su instancia para desactivar esas llamadas de API.</li></td>
  </tr>
  <tr> 
   <td>Adobe Dynamic Chat (si procede)</td> 
<td>Siga los pasos que se indican a continuación para acceder a <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. Si aún no ha configurado un Adobe ID, <a href="https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html" target="_blank">aprenda a hacerlo aquí</a>.
<br/>
<li>¿Ha aceptado la <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Administrador de productos de Dynamic Chat</a> ¿invitar? El correo electrónico se envía cuando Dynamic Chat está habilitado en la instancia de Marketo Engage y usted ha sido designado como administrador del sistema.
<br/>     Si no es así, busque el correo electrónico de bienvenida en la bandeja de entrada y acepte la invitación para configurar su Adobe ID.</li>   
<li>¿Ha añadido el <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">usuarios deseados</a> al perfil de producto Dynamic Chat en Adobe Admin Console?
<li>Asegúrese de que los usuarios aptos tengan el perfil de producto de Dynamic Chat añadido a su identidad de Adobe. No puede asignar funciones de "Dynamic Chat de acceso" en Marketo Engage &gt; Administración &gt; Usuarios y funciones si se añaden a un perfil de producto.</li>
<li>En la pestaña "Perfiles de producto", ¿los permisos de perfil predeterminados están alineados con las necesidades de su organización?<br/> 
Si no es así, edite los permisos del perfil específico. </li>
<li>Si tiene más de una suscripción, ¿se añaden los usuarios a las suscripciones correctas?</li>
<br>
Una vez que haya terminado de auditar la configuración de Usuarios y funciones, inicie sesión en Dynamic Chat para continuar con la auditoría.  
<li>¿Tiene usted <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">conectó su instancia de Marketo Engage</a> al Dynamic Chat?</li>
<li>¿Los cinco perfiles predeterminados con permisos predefinidos son aplicables a su organización?<br/> 
     Si no es así, puede <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">editarlos en Dynamic Chat</a>. También puede <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">crear un perfil personalizado</a> con un conjunto personalizado de permisos.</li>
<li>Para proporcionar a los usuarios acceso a Dynamic Chat, ¿ha marcado "Acceder a Dynamic Chat" para la función de Marketo Engage aplicable en Administración &gt; Usuarios y funciones &gt; Funciones?
<br/><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Los roles "Administrador" y "Usuario de marketing" deben tener acceso a Dynamic Chat.</li>
</td>
  </tr>
  <td>Perspectiva de ventas de Marketo (si corresponde)</td> 
   <td><li>Tiene el <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">Se ha instalado el paquete MSI</a>?</li>
<li>¿Tiene usted <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">actualizado a la última versión de Sales Insight</a>?</li>
<li>¿Ha completado la configuración de Sales Insight? <br/>     Usuarios empresariales/ilimitados <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">haga clic aquí</a>, Usuarios profesionales <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">haga clic aquí</a>.</li>
<li>¿Tiene usted <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">acceso dado a los usuarios</a> ¿en función del número de puestos que has comprado?</li>
<li>Son <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Estrellas y llamas</a> ¿personalizado?</li></td>
  </tr>
  <tr> 
   <td>Punto de inicio (si corresponde)</td> 
   <td><li>Qué servicios ha configurado (por ejemplo, <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a>, etc.)? ¿Están a punto de expirar?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Cuántas llamadas de API</a> ¿utilizan sus integraciones?</li>
<li>¿Tiene las integraciones adecuadas para sus casos de uso?</li></td>
  </tr>
  <tr> 
   <td>Webhooks (si procede)</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Qué conexiones</a> ¿lo has arreglado?</li>
<li>¿Ya no se utiliza alguno?</li></td>
  </tr>
  <tr> 
   <td>Aplicaciones móviles (si corresponde)</td> 
   <td><li>Que <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">aplicaciones móviles</a> ¿tiene usted?</li>
<li>Tener alguna <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">dispositivos de prueba</a>  ¿se ha añadido?</li></td>
  </tr>
 </tbody> 
</table>

## Cofre del tesoro {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Cofre del tesoro</td> 
   <td><li>¿Qué está activado en el? <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">Cofre del tesoro</a>?</li>
<li>¿Hay funciones que se deben activar o desactivar?</li></td>
  </tr>
  <tr> 
   <td>Inspector de campaña</td> 
   <td><li>Es <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Inspector de campaña</a> ¿encendida?
<br/>Si no es así, considere activarla para identificar fácilmente qué campañas están activas, sincronizándose con su CRM o eliminando registros.</li></td>
  </tr>
 </tbody> 
</table>

## Alertas y actualizaciones {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar enfoque</th>
  </tr> 
  <tr> 
   <td>Actualizaciones de estado del Marketo Engage</td> 
   <td><li>¿Está su instancia suscrita a <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Actualizaciones de estado del Marketo Engage</a>?</li></td>
  </tr>
  <tr> 
   <td>Alertas</td> 
   <td><li>¿Hay alguna? <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">alertas activas</a> se envía a los equipos internos desde el Marketo Engage?</li>
<li>En caso afirmativo, ¿funcionan correctamente esas alertas?</li></td>
  </tr>
  <tr> 
   <td>Notificaciones</td> 
   <td><li>¿Está suscrito al administrador correspondiente? <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">notificaciones</a>?</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[Auditoría de una Instancia Heredada: ► de Base de Datos](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/database-checklist.md)
