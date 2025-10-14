---
description: 'Notas de la versión, octubre de 2024: Documentos de Marketo: documentación del producto'
title: Notas de la versión, octubre de 2024
feature: Release Information
exl-id: 2e28ae7f-51de-4510-b3e8-79a989f0daf5
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 21%

---

# Notas de la versión: octubre de 2024 {#release-notes-oct-24}

A continuación encontrará todas las funciones incluidas en la versión de octubre de 2024. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 04 de octubre de 2024**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
    <tr>
   <td><strong>Tokenización para seminarios web interactivos</strong>: ahora puede usar tokens para promocionar seminarios web interactivos en correos electrónicos y páginas de destino sin tener que agregar manualmente los detalles del seminario web.</td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">Promoción de un seminario web interactivo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Recuento de listas inteligentes configuradas para afectar a</strong>: vea cuántas personas se verán afectadas al editar las reglas de calificación de una campaña inteligente.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Botón Mi cuenta en el carril de navegación</strong>: Para aquellos que han migrado a Adobe Identity Management System, un nuevo botón "Mi cuenta" en el carril de navegación izquierdo permite configurar su zona horaria y acceder a los detalles de suscripción.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Mejoras en el informe de rendimiento del correo electrónico</strong>: se han realizado varias mejoras en las métricas de informes de correo electrónico y en el seguimiento de actividades, lo que ofrece perspectivas adicionales y mejora la precisión.
   <ul>
   <li>Filtrar personas eliminadas y combinadas de las métricas de rendimiento de correo electrónico</li>
   <li>Correos electrónicos ahora clasificados como <i>anulados</i> después de esperar tres días para la actividad de respuesta</li>
   <li>Las aperturas de correo electrónico se cuentan como aperturas únicas por separado para cada campaña inteligente</li>
   </td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">Informe de rendimiento de correo electrónico</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Métricas de trabajo pendiente de sincronización de Salesforce</strong>: supervise el rendimiento de sincronización y las tendencias de trabajo pendiente para planificar y programar actualizaciones de CRM para una experiencia de sincronización óptima.
   </td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Métricas de registro de asuntos pendientes de Salesforce</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Actualización de API de extracción masiva**: se ha corregido un problema en la API de extracción masiva que incluía la opción columnHeaderNames, que le permite especificar nombres de encabezado de columna personalizados en el archivo exportado. Anteriormente, los nombres de encabezados de columna que contenían caracteres no ASCII podían dañarse.

* **Desaprobación del parámetro access_token de la API de REST**: El parámetro de consulta &quot;access_token&quot; usado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de enero de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API de REST usando el encabezado &quot;Autorización&quot; [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication#using-an-access-token).

* **Desaprobación del código QR**: El 4 de octubre de 2024, la función de código QR utilizada en las notificaciones push y los recursos de mensajería en la aplicación dejará de usarse. Esto incluye el uso de códigos QR para un nuevo dispositivo de prueba y la creación de nuevos recursos con códigos QR. Las funciones en desuso con un menor uso nos permiten reasignar sus recursos al mantenimiento general de Marketo Engage.

* **Cambios de Munchkin**

   * **Nueva versión**: El 17 de septiembre de 2024, [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 empezará a implementarse en las instancias de Marketo Engage que tengan la configuración &quot;Munchkin Beta&quot; habilitada en **Administración** > **Tesoro**. Está programado para comenzar el despliegue en todas las demás instancias el 29 de octubre. Esta versión actualiza la creación de cookies de Munchkin. No hay cambios en la funcionalidad.

   * **Se eliminaron caracteres de la URL**: Las actividades &#39;Visitas a la página web&#39; y &#39;Clics en el vínculo&#39; creadas por Munchkin JS ahora eliminarán los caracteres de control sin codificación de URL de todos los campos de URL. Este cambio está diseñado para evitar errores relacionados con la propagación de esos tipos de caracteres a sistemas que no los admiten y que no tienen un uso válido en Marketo Engage.
