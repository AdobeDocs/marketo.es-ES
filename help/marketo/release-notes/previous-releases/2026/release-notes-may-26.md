---
description: 'Notas de la versión, mayo de 2026: Documentos de Marketo: documentación del producto'
title: Notas de la versión, mayo de 2026
feature: Release Information
source-git-commit: 7ed34709d2a8b8ab3922a62d043bcdfa8e2d33ce
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 14%

---

# Notas de la versión: mayo de 2026 {#release-notes-may-26}

A continuación encontrará todas las funciones incluidas en la versión de mayo de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **22 de mayo de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Marketo AI</strong>: utilice un conjunto de agentes diseñados para automatizar funciones de marketing importantes pero que requieren mucho tiempo (hay dos agentes disponibles ahora y más próximamente).
</td>
   <td>Abrir versión beta</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/overview" target="_blank">Información general sobre Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Servidor MCP de Marketo Engage</strong>: El servidor MCP de Marketo Engage actúa como un puente entre su asistente de IA y Marketo Engage. Expone más de 100 operaciones en formularios, programas, campañas inteligentes, personas/posibles clientes, correos electrónicos, fragmentos de código, listas y carpetas.</td>
   <td>Abrir versión beta</td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/mcp-server.html" target="_blank">Servidor MCP de Marketo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de correo electrónico - Contenido condicional para fragmentos de correo electrónico</strong>: <i>Paridad con el antiguo editor de correo electrónico</i>. Ahora se admite contenido condicional para los fragmentos.</td>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Administración de listas de selección</strong>: ahora puede especificar los valores que se pueden usar en los campos en Marketo Engage.
   </td>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/administration/field-management/picklist-management.md" target="_blank">Administración de listas de selección</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Está escribiendo</strong>: Ahora tanto el visitante como el agente ven un mensaje "está escribiendo..." mientras la otra parte está escribiendo, evitando que una interrumpa a la otra.</td>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Campos de lista de selección/lista desplegable de Marketo</strong>: Los campos de lista de selección/persona desplegable de Marketo (incluidos los valores sincronizados con Salesforce) ya están disponibles como valores desplegables en el editor de perfiles de chat.
   </td>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Estado de chat perdido</strong>: Cuando un agente no acepta un chat, aparecerá un nuevo estado "Chat perdido" en los Detalles de la actividad en el Registro de persona de la persona que conversó en.
   </td>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Dynamic Chat - Nuevo comportamiento de sincronización de atributos</strong>: Anteriormente, al agregar nuevos atributos, se bloqueaban los cambios en el entorno durante un máximo de 24 horas mientras se completaba la sincronización, lo que impedía la edición y publicación de cuadros de diálogo. Ahora, mientras que la adición de un nuevo atributo requiere una sincronización de datos completa (que puede tardar hasta 24 horas), el entorno ya no se bloquea durante el proceso.</td>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Campos de obsolescencia de funciones sociales**: en 2025, Marketo Engage dejó de utilizar las siguientes funciones sociales:

   * Sondeos
   * Botón social
   * Oferta de referencia
   * Compartir video
   * Sorteos

A principios de este año, los campos relacionados que se habían dejado atrás se eliminaron de Marketo. Poco después, las solicitudes de API que hacían referencia a ciertos campos de posibles clientes relacionados con Social devolvieron un error de &quot;campo no encontrado&quot;, lo que provocó interrupciones. El servicio se restauró después de que los campos afectados volvieran a estar disponibles, por lo que, para evitar más interrupciones, Marketo ha disociado permanentemente los campos de Social de la obsolescencia de las funciones de Social (y, como tales, estarán disponibles en su cuenta de Marketo). Se recomienda a los usuarios revisar las consultas e integraciones de API que hacen referencia a campos relacionados con Marketo Social y determinar si esos campos siguen siendo necesarios para los procesos empresariales en curso.

* **Funcionalidad de combinación de API para campos booleanos**: El comportamiento de los campos booleanos en una combinación de API cambió en la versión de marzo de 2026. Ahora, un valor False se trata correctamente como si tuviera un valor para ese campo. Solo un valor nulo se trata como &quot;vacío&quot; al evaluar campos en conflicto. Vea [esta publicación de la comunidad](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219){target="_blank"} para obtener más información.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de julio de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Límite de posibles clientes de combinación de API REST**: A partir del 31 de julio de 2026, las llamadas que incluyan más de 25 ID en el parámetro leadIds de una llamada de API de combinación de posibles clientes generarán un código de error 1080, y se omitirá la llamada. Los trabajos que requieren la fusión de más de 25 registros en uno deben dividirse en varios trabajos para garantizar el éxito de esas llamadas.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de julio de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos Obtener actividades de posibles clientes y Obtener cambios de posibles clientes que incluyan el parámetro `listId` devolverán un código de error 1003 si la lista estática de destino contiene 10 000 posibles clientes o más. Consulte la [Guía de migración](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener más información.
