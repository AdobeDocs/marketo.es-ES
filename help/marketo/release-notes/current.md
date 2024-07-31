---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: d61ac2c4b7c3fbd138a75b51bb184e4bfd1eef3c
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 7%

---

# Notas de la versión: julio de 2024 {#release-notes-july-24}

A continuación encontrará todas las funciones incluidas en la versión de julio de 2024. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión específicas del Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **26 de julio de 2024**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
     <tr> 
   <td><strong>Tablero de participación para seminarios web interactivos</strong>: obtenga una vista de rendimiento de seminario web agregada, así como una vista completa de la participación de cada asistente durante el seminario web, para que pueda decidir qué clientes potenciales se dirigirán a través de las herramientas de orquestación de Marketo Engage.</td> 
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
   <td><strong>Administración de salas para seminarios web interactivos</strong>: Acceda a las salas individuales creadas (y realice las modificaciones necesarias), así como el contenido y la grabación (y bórrelos si es necesario para optimizar el almacenamiento).</td> 
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
   <td><strong>Personalización de seminarios web para seminarios web interactivos</strong>: proporcione una experiencia de marca aprobada por la organización uniforme mediante el uso de una interfaz de sala común, pantallas intermediarias (como fondos de pantalla de entrada de asistentes) y fondos de vídeo personalizados para que la estrategia de seminario web se pueda alinear más fácilmente con la estrategia de marca.</td> 
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
   <td><strong>Cambio de la API de REST de Marketo</strong>: estamos introduciendo un cambio menor en la <a href="https://developers.marketo.com/rest-api/user-management/">API de administración de usuarios</a>. Los extremos <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Examinar usuarios</a> y <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Eliminar usuario</a> ahora admiten usuarios de <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Administración de cuentas de Target</a>.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Nuevo sitio de documentación para desarrolladores**: Como parte de nuestro esfuerzo continuo por mejorar la experiencia del usuario Marketo Engage, migraremos toda la documentación para desarrolladores al sitio web de Adobe Experience League y Adobe Developer en julio de 2024. [Más información](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Degradación de funciones sociales**: El miércoles 31 de julio de 2024, Marketo Engage empezará a retirar las siguientes funciones sociales del producto:

   * Sondeos
   * Botón social
   * Oferta recomendada
   * Compartir video
   * Sorteos

Los usuarios ya no podrán crear, clonar ni incrustar ninguna de estas funciones de Social en Marketo Engage. Los recursos sociales existentes seguirán funcionando hasta el 31 de enero de 2025. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Token de acceso en desuso del parámetro de consulta**: La compatibilidad con la autenticación mediante tokens de acceso en un parámetro de consulta de una llamada de API de REST de Marketo Engage se eliminará en una versión futura (fecha específica por determinar). Las integraciones existentes deberían migrar al uso del encabezado de autorización [descrito aquí](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. El nuevo desarrollo solo debe utilizar el encabezado Autorización para la autenticación con el Marketo Engage.

* **Se requiere reautenticación de LinkedIn**: LinkedIn está actualizando sus API de marketing utilizadas por las integraciones de Marketo Engage LinkedIn. Estos cambios requerirán la reautenticación de todos los servicios LaunchPoint de LinkedIn en su menú de **Admin** > **LaunchPoint** entre el 26 de julio y el 15 de diciembre de 2024 para evitar la interrupción del servicio. Puede encontrar instrucciones sobre cómo lograr este(a) [aquí para la generación de clientes potenciales Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} y [aquí para las audiencias coincidentes](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. El servicio de formularios de generación de clientes potenciales tiene un tipo de &quot;LinkedIn Lead Gen&quot; y el servicio de audiencias coincidentes tiene un tipo de &quot;LinkedIn Matched Audiences&quot;. Para obtener más información, consulte las [Preguntas frecuentes sobre la migración](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
