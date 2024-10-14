---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ef1cb0b67deb935b67a56076ed9ed0a14f449662
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 5%

---

# Notas de la versión: octubre de 2024 {#release-notes-oct-24}

A continuación encontrará todas las funciones incluidas en la versión de octubre de 2024. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión específicas del Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **4 de octubre de 2024**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
    <tr> 
   <td><strong>Datos de registro mejorados en el panel de participación para seminarios web interactivos</strong>: ahora puede ver qué compañías han tenido la mayor asistencia y obtener información sobre la compañía, el título y el sector a nivel de posible cliente en los informes disponibles en el panel de participación.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
    <tr> 
   <td><strong>Tokenización para seminarios web interactivos</strong>: ahora puede usar tokens para promocionar seminarios web interactivos en correos electrónicos y páginas de destino sin tener que agregar manualmente los detalles del seminario web.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
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
   <td>n/a</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>Botón Mi cuenta en el carril de navegación</strong>: Para aquellos que han migrado a Adobe Identity Management System, un nuevo botón "Mi cuenta" en el carril de navegación izquierdo permite configurar su huso horario y acceder a los detalles de la suscripción.</td> 
   <td>Enviado</td>
   <td>n/a</td>
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
   <li>Se ha mejorado el seguimiento de la actividad de correo electrónico mediante el refinamiento de la ubicación del píxel de seguimiento</li>
   </td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">Informe de rendimiento de correo electrónico</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Desaprobación del código QR**: El 4 de octubre de 2024, la función de código QR utilizada en las notificaciones push y los recursos de mensajería en la aplicación dejará de usarse. Esto incluye el uso de códigos QR para un nuevo dispositivo de prueba y la creación de nuevos recursos con códigos QR. Las funciones en desuso con un menor uso nos permiten reasignar sus recursos al mantenimiento general de Marketo Engage.

* **Cambios de Munchkin**

   * **Nueva versión**: El 17 de septiembre de 2024, [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 empezará a implementarse en las instancias de Marketo Engage que tengan la configuración &quot;Munchkin Beta&quot; habilitada en **Administración** > **Cofre del tesoro**. Está programado para comenzar el despliegue en todas las demás instancias el 29 de octubre. Esta versión actualiza la creación de cookies de Munchkin. No hay cambios en la funcionalidad.

   * **Se eliminaron caracteres de la URL**: Las actividades &#39;Visitas a la página web&#39; y &#39;Clics en el vínculo&#39; creadas por Munchkin JS ahora eliminarán los caracteres de control sin codificación de URL de todos los campos de URL. Este cambio está diseñado para evitar errores relacionados con la propagación de esos tipos de caracteres a sistemas que no los admiten y que no tienen un uso válido dentro de Marketo Engage.
