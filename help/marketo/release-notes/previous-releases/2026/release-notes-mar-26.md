---
description: 'Notas de la versión, marzo de 2026: Documentos de Marketo: documentación del producto'
title: Notas de la versión, febrero de 2026
feature: Release Information
source-git-commit: 713ab854749cb88a35b24f4355368092cdb35e64
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 21%

---

# Notas de la versión: marzo de 2026 {#release-notes-mar-26}

A continuación encontrará todas las funciones incluidas en la versión de marzo de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **27 de marzo de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Correo electrónico de Designer - Administrar marcas (beta)</strong>: genere contenido de correo electrónico en función de las directrices de redacción específicas de su organización o marca.</td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/manage-brands.md" target="_blank">Crear y administrar marcas</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Componentes editables de HTML en fragmentos</strong>: en los fragmentos visuales, los campos editables son compatibles con los componentes de imagen, texto y botones a través del panel de propiedades del componente. Para los componentes de HTML, los campos editables se configuran de forma diferente, utilizando una sintaxis basada en variables dentro del código fuente del propio componente de HTML.
   </td>
   <td>Publicado</i></td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/customizable-fragments#editable-html" target="_blank">Componentes editables de HTML en fragmentos</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Acciones rápidas</strong>: <i>Paridad con el antiguo editor de correo electrónico</i>. Ahora hay acciones rápidas disponibles para todos los recursos de Designer de correo electrónico (correos electrónicos, plantillas de correo electrónico, fragmentos). Las acciones rápidas admitidas son: Duplicar, Eliminar, Mover, Crear/Editar borrador.
   </td>
   <td>Publicado</i></td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Email Designer - Corrección de procesamiento de Outlook</strong>: Esta actualización corrige los problemas de procesamiento, especialmente en MS Outlook. El modo avanzado de HTML le permite realizar pequeñas ediciones de HTML/CSS o añadir etiquetas de script a la plantilla de correo electrónico.
   </td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/advanced-html-mode.md" target="_blank">Edición de plantillas de correo electrónico con el editor avanzado de HTML</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Comprobador de puntuación de marca</strong>: evalúe la calidad general del contenido para identificar posibles problemas con legibilidad, coherencia del contenido y eficacia, independientemente de las directrices de marca.</td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/brand-score.md" target="_blank">Puntuación de marca</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Notificaciones push</strong>: Los URI de redireccionamiento configurados en los mensajes de notificaciones push ahora admiten tokens de Marketo Engage (aplicable solo a <i>URL de aplicaciones de Launch</i>).
   </td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md#redirect-uris">URI de redireccionamiento</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Desaprobación de la característica SEO**: El martes 31 de marzo de 2026, Marketo Engage dejará de utilizar la característica de optimización del motor de búsqueda (SEO). Si no usas SEO de forma activa, no tienes que hacer nada. Si ha utilizado recientemente el SEO, tiene la opción de exportar los datos. [Más información](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}.

* **Límite de posibles clientes de combinación de API REST**: A partir del 31 de julio de 2026, las llamadas que incluyan más de 25 ID en el parámetro leadIds de una llamada de API de combinación de posibles clientes generarán un código de error 1080, y se omitirá la llamada. Los trabajos que requieren la fusión de más de 25 registros en uno deben dividirse en varios trabajos para garantizar el éxito de esas llamadas.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de julio de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de julio de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
