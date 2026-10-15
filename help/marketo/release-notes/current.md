---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: 'https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 9eb8c0e78a581bc9093f0f017a3ad3525d2b9667
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 18%
---
# Notas de la versión: octubre de 2026 {#release-notes-oct-26}

A continuación encontrará todas las funciones incluidas en la versión de octubre de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **23 de octubre de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Clonar a este programa/carpeta</strong>: Las operaciones de clonación en Marketo Engage ahora ofrecen de forma consistente una opción "Esta carpeta" o "Este programa" como primera opción al elegir el destino del recurso clonado. Al elegir esta opción, se clona el recurso en el programa o la carpeta principal del recurso actual.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <tr>
   <td><strong>Alerta instantánea en la sincronización con CRM</strong>: al habilitar o deshabilitar la sincronización de CRM nativa para un entorno, ahora se envía una déclencheur a los usuarios suscritos al canal de notificación de CRM.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Desuso de Capturar imágenes de la web**: Para ajustarse a las prácticas recomendadas modernas de seguridad y privacidad, la función [Capturar imágenes de la web](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} quedará obsoleta a partir de la versión de octubre.

* **Restricciones de nombres de API para atributos de actividad personalizados**: Los nombres de API para atributos de actividad personalizados creados mediante la API o la interfaz de usuario ahora solo pueden contener caracteres alfanuméricos y guiones bajos, y deben comenzar con un carácter alfanumérico.

* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos de obtener actividades de posibles clientes u obtener cambios de posibles clientes que incluyen el parámetro `listId` comenzaron a fallar con un código de error 1003 (que indica que la lista estática de destino tiene demasiados registros) si las listas de destino contienen 10 000 posibles clientes o más. Consulte la [Guía de migración](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener información adicional.
