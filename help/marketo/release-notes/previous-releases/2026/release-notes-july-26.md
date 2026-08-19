---
description: 'Notas de la versión, julio de 2026: Documentos de Marketo: documentación del producto'
title: Notas de la versión, julio de 2026
feature: Release Information
source-git-commit: 37ef6b0f6c89b8ec8cd098beb5cf4d321fdac401
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 19%

---

# Notas de la versión: julio de 2026 {#release-notes-july-26}

A continuación encontrará todas las funciones incluidas en la versión de julio de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **10 de julio de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Habilidad de Marketo AI - Conocimiento del producto</strong>: El conocimiento del producto le brinda acceso a petición a la experiencia de Marketo sin salir de la plataforma. Haga una pregunta en lenguaje sencillo y Marketo AI utiliza la documentación oficial de Adobe para proporcionar una respuesta.
</td>
   <td>Publicado</td>
   <td><a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Conocimiento del producto</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Habilidad de Marketo AI: investigar posibles clientes</strong>: descubra por qué una persona o posible cliente específico no alcanzó un hito (como MQL, calificación de programas o una campaña) y obtenga una explicación en lenguaje sencillo de lo que sucedió.
</td>
   <td>Publicado</td>
   <td><a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Investigar posibles clientes</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Módulos</strong>: Ahora tiene acceso a bloques de contenido totalmente estructurados y listos para usar diseñados para acelerar el ensamblado de correo electrónico.</td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/email-modules.md" target="_blank">Uso de módulos de en el Designer de correo electrónico</a></td>
  </tr>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Generate Content Contextual Menu</strong>: Ahora se puede acceder a las funciones "Generar contenido" de Email Designer desde el menú contextual (la barra negra). Por ejemplo, al seleccionar contenido de texto, el icono Generar contenido aparece en el menú contextual, lo que le permite realizar acciones rápidas.</td>
   <td><i>Próximamente</i></td>
<td><i>Próximamente</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de agosto de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.
* **Límite de posibles clientes de combinación de API REST**: A partir del 31 de julio de 2026, las llamadas que incluyan más de 25 ID en el parámetro leadIds de una llamada de API de combinación de posibles clientes generarán un código de error 1080, y se omitirá la llamada. Los trabajos que requieren la fusión de más de 25 registros en uno deben dividirse en varios trabajos para garantizar el éxito de esas llamadas.
* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de julio de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos Obtener actividades de posibles clientes y Obtener cambios de posibles clientes que incluyan el parámetro `listId` devolverán un código de error 1003 si la lista estática de destino contiene 10 000 posibles clientes o más. Consulte la [Guía de migración](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener más información.
