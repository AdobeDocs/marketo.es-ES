---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
hide: true
hidefromtoc: true
feature: Release Information
source-git-commit: 38ec4726dece1695a15104fdb7fa7592b298d4a9
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 7%

---

# Notas de la versión: abril de 2025 {#release-notes-apr-25}

A continuación encontrará todas las funciones incluidas en la versión de abril de 2025. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **25 de abril de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Función</th> 
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr> 
   <td><strong>Compatibilidad de plantillas para Designer de correo electrónico</strong>: Las plantillas de correo electrónico del editor de correo electrónico clásico ahora son compatibles con el nuevo <a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Designer de correo electrónico</a>.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Autoservicio de capa de sockets seguros (SSL)</strong>: el cifrado SSL le permite hacer que las páginas de aterrizaje de una instancia de Marketo Engage sean seguras. Para habilitar esta función se necesitaba la asistencia del equipo de asistencia de Adobe. Los usuarios de Marketo ahora pueden habilitarlo por su cuenta, lo que ahorra un tiempo valioso.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Nueva característica de Analytics - Beta público**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anteriormente conocido como Revenue Explorer y Advanced Report Builder) comienza a implementarse para todos los usuarios actuales del Revenue Cycle Explorer a mediados de abril. Esta nueva herramienta ofrece una interfaz flexible de creación de informes y visualización en datos de Marketo Engage, que proporciona detalles granulares sobre progresión, rendimiento, etc. Ofrece una mejor interactividad y visualización, un rendimiento más rápido y una experiencia de usuario más fluida e intuitiva.

Para acceder a esta función, debe haber adquirido el complemento de Analytics de BI avanzado. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 30 de junio de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API de REST usando el encabezado &quot;Autorización&quot; [tal como se describe aquí](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de octubre de 2025. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API de REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Desaprobación de funciones sociales**: El miércoles 31 de julio de 2024, Marketo Engage comenzó la desaprobación de las siguientes funciones sociales del producto:

   * Sondeos
   * Botón social
   * Oferta recomendada
   * Compartir video
   * Sorteos

A partir de ese momento, los usuarios no han podido crear, clonar ni incrustar ninguna de estas funciones de Social en Marketo Engage. Los recursos sociales existentes seguirán funcionando hasta el 31 de enero de 2025. El 1 de febrero de 2025, los activos sociales dejaron de funcionar. Deberá eliminar cualquier función social incrustada en las páginas de destino. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
