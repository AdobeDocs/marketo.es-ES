---
description: 'Notas de la versión actuales, Documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 0d2416651da183460ad1f60ff5d566cbfc7abd12
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 10%

---

# Notas de la versión: abril de 2024 {#release-notes-apr-24}

A continuación encontrará todas las funciones incluidas en la versión de abril de 2024. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión se han diseñado específicamente para Adobe Dynamic Chat [se puede encontrar aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![estrella](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes funciones entran dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **26 de abril de 2024**, con un despliegue gradual de las funciones restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
     <tr> 
   <td><strong>Mejoras en seminarios web interactivos</strong>: ahora puede proporcionar a los hosts y moderadores la capacidad de añadir un título de seminario web, cambiar el nombre de una sala y sincronizar manualmente los datos de participación después de la entrega del evento.</td> 
   <td>Enviado</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Crear un seminario web interactivo</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Sincronización manual</a></li></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Mejoras de pista de auditoría</strong>: Ahora se pueden capturar nuevos tipos de acciones en la pista de auditoría para los cambios realizados en Administración de campos, los cambios realizados en Usuarios y funciones y el recuento de personas exportadas desde listas y listas inteligentes.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Nuevos permisos de usuarios y funciones</strong>: Hay nuevos permisos disponibles, que proporcionan a los usuarios un acceso más granular a Marketo Engage. Controle las partes del administrador que no estaban bloqueadas anteriormente, como Nueva experiencia y Audiencias predictivas, divida los permisos para conceder acceso a la pista de auditoría de recursos y a la pista de auditoría de administración por separado y utilice los nuevos permisos de creación y movimiento de recursos y carpetas para evitar que los usuarios de solo lectura realicen cambios. 
   <p>Aunque los nuevos permisos aparecerán en la instancia de Marketo Engage a partir del 26 de abril, por ahora son pasivos y estarán accesibles a finales de este trimestre.
   <li>Acceso a Adobe Experience Manager</li>
   <li>Asignación de organización de Adobe de acceso</li>
   <li>Registro de auditoría de administración de acceso</li>
   <li>Acceder a pista de auditoría de activos</li>
   <li>Acceder a nueva experiencia</li>
   <li>Acceso a Predictive Audiences</li>
   <li>Crear informe</li>
   <li>Crear lista</li>
   <li>Exportar actividad de campaña</li>
   </td> 
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Descripciones de los permisos de funciones</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Actualización de API de actividades**: El 26 de abril, añadiremos varios atributos nuevos a las actividades basadas en la web y en correo electrónico que se devuelven cuando recupera actividades mediante [API DE REST DE MARKETO](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} extremo para revisar los detalles de atributos de cada actividad.

**Actividades basadas en Web**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Actividad</th> 
   <th style="width:70%">Atributos añadidos recientemente</th>
   </tr>
  <tr> 
   <td>Visit Webpage</td> 
   <td>Explorador, plataforma y dispositivo</td>
  </tr>
   <tr> 
   <td>Completar formulario</td> 
   <td>Explorador, plataforma y dispositivo</td>
  </tr>
  <tr> 
   <td>Haga clic en Vínculo</td> 
   <td>Explorador, plataforma y dispositivo</td>
  </tr>
 </tbody> 
</table>

**Actividades basadas en correo electrónico**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Actividad</th> 
   <th style="width:70%">Atributos añadidos recientemente</th>
  </tr>
   <tr> 
   <td>Enviar email</td> 
   <td>Explorador, plataforma, dispositivo, agente de usuario</td>
  </tr>
   </tr>
  <tr> 
   <td>Email entregado</td> 
   <td>Explorador, plataforma, dispositivo, agente de usuario</td>
  </tr>
   <tr> 
   <td>Se rechazó el email</td> 
   <td>Explorador, plataforma, dispositivo, agente de usuario</td>
  </tr>
  <tr> 
   <td>Cancelar suscripción a los correos electrónicos</td> 
   <td>Explorador, plataforma y dispositivo</td>
  </tr>
  <tr> 
   <td>Abrir correo electrónico</td> 
   <td>Navegador</td>
  </tr>
   <tr> 
   <td>Hacer clic en el correo electrónico</td> 
   <td>Navegador</td>
  </tr>
  <tr> 
   <td>Se rechazó temporalmente el email</td> 
   <td>Explorador, plataforma, dispositivo, agente de usuario</td>
  </tr>
 </tbody> 
</table>
