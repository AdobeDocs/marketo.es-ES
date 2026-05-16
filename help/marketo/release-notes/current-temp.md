---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
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
source-git-commit: a04ec3931933c8e6cc0a0ffc26b1b559cd7cc9ce
workflow-type: tm+mt
source-wordcount: 421
ht-degree: 28%

---

# Notas de la versión: mayo de 2026 {#release-notes-may-26}

A continuación encontrará todas las funciones incluidas en la versión de mayo de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

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
   <td><strong>Designer de correo electrónico - Contenido condicional para fragmentos de correo electrónico</strong>: <i>Paridad con el antiguo editor de correo electrónico</i>. Ahora se admite contenido condicional para los fragmentos.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Administración de listas de selección</strong>: ahora puede especificar los valores que se pueden usar en los campos en Marketo Engage.
   </td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
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

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de julio de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de julio de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos Obtener actividades de posibles clientes y Obtener cambios de posibles clientes que incluyan el parámetro `listId` devolverán un código de error 1003 si la lista estática de destino contiene 10 000 posibles clientes o más. Consulte la [Guía de migración](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener más información.
