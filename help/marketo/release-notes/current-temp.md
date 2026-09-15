---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
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
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: df650f93bedc7202ad82f8f725616cd25e4a99ef
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 18%
---
# Notas de la versión: septiembre de 2026 {#release-notes-sep-26}

A continuación encontrará todas las funciones incluidas en la versión de septiembre de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **25 de septiembre de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Nueva interfaz de usuario de Marketo Engage</strong>: La interfaz de Marketo Engage tiene un aspecto actualizado, que incluye menús, iconos y diseño actualizados para una experiencia más limpia y moderna. Esto es solo una actualización visual; no afecta a la funcionalidad ni a los flujos de trabajo existentes. <i>La capacidad de seleccionar la IU clásica estará disponible hasta la versión de enero de 2027</i>.
</td>
   <td>Disponibilidad general a finales de septiembre</td>
   <td><i>n/a</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Seleccionar partición al importar</strong>: ahora puede seleccionar de la lista de particiones del espacio de trabajo local al importar registros de personas en entornos que tienen espacios de trabajo y particiones habilitados.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Alerta instantánea en la sincronización CRM</strong>: Los usuarios suscritos a las notificaciones de CRM recibirán una notificación inmediata cuando cambie el estado habilitado de su sincronización nativa de CRM, lo que proporcionará a los administradores mayor visibilidad de su estado de sincronización de CRM.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Pasos de flujo de autoservicio - Tiempo de espera de devolución de llamada aumentado</strong>: El tiempo de espera de devolución de llamada para los pasos de flujo de autoservicio se está incrementando de una hora a cuatro horas. No se requiere ninguna acción por su parte.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Restricciones de nombres de API para atributos de actividad personalizados**: Los nombres de API para atributos de actividad personalizados creados mediante la API o la interfaz de usuario ahora solo pueden contener caracteres alfanuméricos y guiones bajos, y deben comenzar con un carácter alfanumérico.

* **Límites de tamaño de lista estática para obtener actividades de posibles clientes y obtener cambios de posibles clientes**: a partir del 30 de septiembre de 2026, las llamadas a los extremos de obtener actividades de posibles clientes u obtener cambios de posibles clientes que incluyan el parámetro `listId` generarán un error de código de error 1003 (que indica que la lista estática de destino tiene demasiados registros) si las listas de destino contienen 10 000 posibles clientes o más. Consulte la [Guía de migración](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obtener información adicional.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo quedó obsoleto el 31 de agosto de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Id. de ejecución de campaña de API REST**: En determinadas circunstancias, el valor del Id. de ejecución de campaña de una actividad se devolvió a veces con un formato incorrecto, entre dos pares de comillas (por ejemplo, `"campaignRunId": ""102938""`).<br/>A partir de la versión de agosto, este valor siempre se devolverá con el formato numérico correcto (`"campaignRunId": 102938`).

* **Desuso de Capturar imágenes de la web**: Para ajustarse a las prácticas recomendadas modernas de seguridad y privacidad, la función [Capturar imágenes de la web](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} quedará obsoleta a partir de la versión de octubre.
