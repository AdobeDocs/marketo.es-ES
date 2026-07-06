---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 14cdc585c2c5b972dd3743c5eb3e253a8a91f608
workflow-type: tm+mt
source-wordcount: 481
ht-degree: 22%

---

# Notas de la versión: 2 de julio #1 2026 {#release-notes-july-26-one}

A continuación encontrará todas las funciones incluidas en la primera versión de julio de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

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
   <td><strong>Habilidad de Marketo AI - Conocimiento del producto</strong>: El conocimiento del producto le brinda acceso a petición a la experiencia de Marketo sin salir de la plataforma. Haga una pregunta en lenguaje sencillo y Marketo AI utiliza la documentación oficial de Adobe para responderla.</td>
   <td>Abrir versión beta</td>
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
   <td>Abrir versión beta</td>
   <td><a href="https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Investigar posibles clientes</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Menú contextual del Asistente de IA</strong>: Ahora se puede acceder a las funciones del Asistente de IA del Designer de correo electrónico desde el menú contextual (la barra negra). Por ejemplo, al seleccionar contenido de texto, el icono Asistente de IA aparece en el menú contextual, lo que le permite realizar acciones rápidas desde allí.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de julio de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Límite de posibles clientes de combinación de API REST**: A partir del 31 de julio de 2026, las llamadas que incluyan más de 25 ID en el parámetro leadIds de una llamada de API de combinación de posibles clientes generarán un código de error 1080, y se omitirá la llamada. Los trabajos que requieren la fusión de más de 25 registros en uno deben dividirse en varios trabajos para garantizar el éxito de esas llamadas.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de julio de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos Obtener actividades de posibles clientes y Obtener cambios de posibles clientes que incluyan el parámetro `listId` devolverán un código de error 1003 si la lista estática de destino contiene 10 000 posibles clientes o más. Consulte la [Guía de migración](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener más información.
