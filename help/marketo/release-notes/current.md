---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2b3c872bfdef4b5cd8e80f754609dd0059c164b2
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 21%

---

# Notas de la versión: agosto de 2026 {#release-notes-aug-26}

A continuación encontrará todas las funciones incluidas en la versión de agosto de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **14 de agosto de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Nueva interfaz de usuario de Marketo Engage</strong>: La interfaz de Marketo Engage tiene un aspecto actualizado, que incluye menús, iconos y diseño actualizados para una experiencia más limpia y moderna. Se trata de una actualización visual; no afecta a la funcionalidad ni a los flujos de trabajo existentes.
</td>
   <td>Despliegue gradual durante todo el mes de agosto</td>
   <td><i>n/a</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Generador de scripts</strong>: El creador de scripts es un asistente con tecnología de IA que le ayuda a crear scripts de personalización más rápido.
</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Deshabilitar campañas en el archivo</strong>: al archivar una carpeta, ahora se deshabilitan y desprograman todas las campañas de ese árbol de carpetas, lo que evita la ejecución inesperada de campañas inteligentes archivadas.
</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de agosto de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Id. de ejecución de campaña de API REST**: En determinadas circunstancias, el valor del Id. de ejecución de campaña de una actividad se devolvió a veces con un formato incorrecto, entre dos pares de comillas (por ejemplo, `"campaignRunId": ""102938""`).<br/>A partir de la versión de agosto, este valor siempre se devolverá con el formato numérico correcto (`"campaignRunId": 102938`)

* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos Obtener actividades de posibles clientes u Obtener cambios de posibles clientes que incluyan el parámetro `listId` fallarán si las listas de destinatarios contienen 10 000 posibles clientes o más con un código de error 1003 que indique que la lista estática de destinatarios tiene demasiados registros.

Consulte la [Guía de migración](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener información adicional.

* **Límite de posibles clientes de combinación de API de REST**: El 31 de julio de 2026, las llamadas que incluyen más de 25 ID en el parámetro leadIds de una llamada de API de Merge Leads generarán un código de error 1080, y se omitirá la llamada. Los trabajos que requieren la fusión de más de 25 registros en uno deben dividirse en varios trabajos para garantizar el éxito de esas llamadas.
