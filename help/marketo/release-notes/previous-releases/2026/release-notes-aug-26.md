---
description: 'Notas de la versión, julio de 2026: Documentos de Marketo: documentación del producto'
title: Notas de la versión, julio de 2026
feature: Release Information
source-git-commit: 15308a78867253ae6c54faa8e77c2cf7eb68b9a5
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 13%
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
   <td><strong>Nueva interfaz de usuario de Marketo Engage</strong>: La interfaz de Marketo Engage tiene un aspecto actualizado, que incluye menús, iconos y diseño actualizados para una experiencia más limpia y moderna. Esto es solo una actualización visual; no afecta a la funcionalidad ni a los flujos de trabajo existentes.
</td>
   <td>Despliegue gradual durante agosto y septiembre</td>
   <td><i>n/a</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Servidor MCP de Marketo Engage</strong>: El servidor MCP de Marketo Engage actúa como un puente entre su asistente de IA y Marketo Engage. Expone más de 100 operaciones en formularios, programas, campañas inteligentes, personas/posibles clientes, correos electrónicos, fragmentos de código, listas y carpetas.</td>
   <td>Disponible de forma general</td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/mcp-server.html" target="_blank">Servidor MCP de Marketo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Deshabilitar campañas en el archivo</strong>: al archivar una carpeta, ahora se deshabilitan y desprograman todas las campañas de ese árbol de carpetas, lo que evita la ejecución inesperada de campañas inteligentes archivadas.
</td>
   <td>Publicado</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders#disable-campaigns-archive" target="_blank">Deshabilitar campañas en el archivo</a></td>
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
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Marketo AI es ahora Coworker para Marketo Engage**: Coworker para Marketo Engage ofrece habilidades de agente diseñadas para automatizar funciones de marketing que consumen tiempo. Nuevo nombre, mismas características, disponible para todos los usuarios. [Más información](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de agosto de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Id. de ejecución de campaña de API REST**: En determinadas circunstancias, el valor del Id. de ejecución de campaña de una actividad se devolvió a veces con un formato incorrecto, entre dos pares de comillas (por ejemplo, `"campaignRunId": ""102938""`).<br/>A partir de la versión de agosto, este valor siempre se devolverá con el formato numérico correcto (`"campaignRunId": 102938`)

* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos de obtener actividades de posibles clientes u obtener cambios de posibles clientes que incluyan el parámetro `listId` generarán un error de código de error 1003 (que indica que la lista estática de destino tiene demasiados registros) si las listas de destino contienen 10 000 posibles clientes o más. Consulte la [Guía de migración](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener información adicional.

* **Límite de posibles clientes de combinación de API de REST**: El 31 de julio de 2026, las llamadas que incluyen más de 25 ID en el parámetro leadIds de una llamada de API de Merge Leads generarán un código de error 1080, y se omitirá la llamada. Los trabajos que requieren la fusión de más de 25 registros en uno deben dividirse en varios trabajos para garantizar el éxito de esas llamadas.
