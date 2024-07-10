---
description: 'Notas de la versión actuales, Documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cb69844d8e9e25cae19bc2d4a91c28376f58eadb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 6%

---

# Notas de la versión: julio de 2024 {#release-notes-july-24}

A continuación encontrará todas las funciones incluidas en la versión de julio de 2024. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión se han diseñado específicamente para Adobe Dynamic Chat [se puede encontrar aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![estrella](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes funciones entran dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **26 de julio de 2024**, con un despliegue gradual de las funciones restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
     <tr> 
   <td><strong>Tablero de participación para seminarios web interactivos</strong>: obtenga una vista agregada del rendimiento del seminario web, así como una vista completa de la participación de cada asistente durante el seminario web, para que pueda decidir qué posibles clientes se dirigirán a través de las herramientas de orquestación del Marketo Engage.</td> 
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
   <td><strong>Administración de salas para seminarios web interactivos</strong>: Acceda a las salas individuales creadas (y realice modificaciones si es necesario), así como acceder al contenido y la grabación (y límpielas si es necesario para optimizar el almacenamiento).</td> 
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
   <td><strong>Personalización de seminarios web para seminarios web interactivos</strong>: proporcione una experiencia de marca aprobada por la organización uniforme mediante el uso de una interfaz de sala común, pantallas intermediarias (como fondos de pantalla de entrada de asistentes) y fondos de vídeo personalizados, para que la estrategia de seminario web se pueda alinear más fácilmente con la estrategia de marca.</td> 
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
   <td><strong>Cambio de API de REST de Marketo</strong>: Presentamos un cambio menor en el <a href="https://developers.marketo.com/rest-api/user-management/">API de administración de usuarios</a>. Tanto la <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Examinar usuarios</a> y <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Eliminar usuario</a> los puntos de conexión ahora admiten <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Administración de cuentas de Target</a> usuarios.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Nuevo sitio de documentación para desarrolladores**: Como parte de nuestro esfuerzo continuo por mejorar la experiencia del usuario Marketo Engage, en julio de 2024 migraremos toda la documentación para desarrolladores al sitio web de Adobe Experience League y Adobe Developer. [Más información](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Token de acceso en desaprobación del parámetro de consulta**: La compatibilidad con la autenticación mediante tokens de acceso en un parámetro de consulta de una llamada de API de REST de Marketo Engage se eliminará en una versión futura (fecha específica por determinar). Las integraciones existentes deben migrar al uso del encabezado Autorización [descrito aquí](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. El nuevo desarrollo solo debe utilizar el encabezado Autorización para la autenticación con el Marketo Engage.

* **Se requiere reautenticación de linkedIn**: LinkedIn está actualizando sus API de marketing utilizadas por las integraciones de Marketo Engage LinkedIn. Estos cambios requerirán volver a autenticar todos los servicios de LaunchPoint de LinkedIn en su **Administrador** > **LaunchPoint** entre el 26 de julio y el 15 de diciembre de 2024 para evitar la interrupción del servicio. Puede encontrar instrucciones sobre cómo hacerlo [aquí para Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} y [aquí para audiencias coincidentes](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. El servicio de formularios de generación de clientes potenciales tiene un tipo de &quot;LinkedIn Lead Gen&quot; y el servicio de audiencias coincidentes tiene un tipo de &quot;LinkedIn Matched Audiences&quot;. Para obtener más información, consulte la [Preguntas frecuentes sobre migración](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
