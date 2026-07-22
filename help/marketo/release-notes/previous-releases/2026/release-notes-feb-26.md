---
description: 'Notas de la versión, febrero de 2026: Documentos de Marketo: documentación del producto'
title: Notas de la versión, febrero de 2026
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: e8663ada66948bc30ff7ad90b26f6ba75d670ae8
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 22%

---

# Notas de la versión: febrero de 2026 {#release-notes-feb-26}

A continuación encontrará todas las funciones incluidas en la versión de febrero de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **20 de febrero de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Acciones de carpeta</strong>: paridad con el antiguo editor de correo electrónico.
   <ul>
   <li>Compartir y archivar acciones de carpeta para recursos de Email Designer.</li>
   <li>Compartir carpetas en espacios de trabajo, hacer clic con el botón derecho en una carpeta para crear un nuevo recurso y mover recursos mediante arrastrar y soltar.</li>
   </ul>
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
   <td><strong>Designer de correo electrónico - API</strong>: Ahora puede usar llamadas de API para el Designer de correo electrónico.</td>
   <td>Publicado</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/asset#">API de recursos Marketo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Correo electrónico de Designer - Generación de imágenes del Asistente de IA</strong>: Ahora, además de Firefly, puede usar modelos de Nano Banana para generar imágenes con el Asistente de IA para el contenido de correo electrónico.</td>
   <td>Publicado</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">Creación de contenido para una sección específica del correo electrónico</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Desaprobación de la característica SEO**: El martes 31 de marzo de 2026, Marketo Engage dejará de utilizar la característica de optimización del motor de búsqueda (SEO). Si no usas SEO de forma activa, no tienes que hacer nada. Si ha utilizado recientemente el SEO, tiene la opción de exportar los datos. [Más información](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}.

* **Límite de posibles clientes de combinación de API REST**: A partir del 31 de julio de 2026, las llamadas que incluyan más de 25 ID en el parámetro leadIds de una llamada de API de combinación de posibles clientes generarán un código de error 1080, y se omitirá la llamada. Los trabajos que requieren la fusión de más de 25 registros en uno deben dividirse en varios trabajos para garantizar el éxito de esas llamadas.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de agosto de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de julio de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
