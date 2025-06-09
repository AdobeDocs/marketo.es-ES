---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 5bd67c4692ed6a383597947fa40d83947f4ca9ff
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 6%

---

# Notas de la versión: mayo de 2025 {#release-notes-may-25}

A continuación encontrará todas las funciones incluidas en la versión de mayo de 2025. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

Las notas de la versión específicas de Adobe Dynamic Chat [ se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características caen dentro del ciclo de lanzamiento estándar y comenzarán a lanzarse el **23 de mayo de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

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
   <td><strong>Tokens de Déclencheur para cualquier atributo</strong>: Se ha ampliado la lista de tokens de déclencheur para admitir el uso de datos de cualquier atributo de actividad en los campos de Smart Campaign.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Contenido de correo electrónico Personalization</strong>: Marketo Engage ahora sigue la misma sintaxis de mayúsculas y minúsculas que los demás tokens de aplicaciones de AEP, por lo que se proporciona una experiencia coherente en todos los productos Adobe DX. Todos los tokens estándar, así como los tokens específicos de Marketo Engage como Miembro, Programa y Mis tokens, están disponibles en el nuevo Designer de correo electrónico.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Control de acceso basado en roles para Designer Assets de correo electrónico</strong>: una nueva mejora del sistema de control de acceso basado en roles (RBAC) proporciona permisos más granulares y una administración de usuarios mejorada para los recursos con tecnología del nuevo Designer de correo electrónico.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Clonación de correos electrónicos creados en el Designer de correo electrónico</strong>: ahora puede clonar un correo electrónico existente creado con el nuevo Designer de correo electrónico.</td> 
   <td>Enviado</td>
   <td>n/a</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Integración de GenStudio en el Designer de correo electrónico</strong>: integre GenStudio para el marketing de rendimiento desde correos electrónicos para mejorar la eficacia del marketing y mantener la coherencia de la marca.</td> 
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anuncios {#announcements}

* **Actualización de integración de conversión sin conexión de Facebook**: El 29 de mayo de 2025, la integración de [Conversión sin conexión de Facebook](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"} para Marketo Engage se migrará a la nueva API de metaconversión [Conversiones](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}, debido a que Meta dejó de utilizar la [API de conversiones sin conexión](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} en línea con el control de versiones de la API de gráficos. Para obtener más información, consulte la guía de Meta sobre [envío de eventos sin conexión a través de la API de conversiones](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI para sin conexión).

* **Nueva característica de Analytics - Beta público**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anteriormente conocido como Revenue Explorer y Advanced Report Builder) comenzó a implementarse para todos los usuarios actuales del Revenue Cycle Explorer a mediados de abril. Esta nueva herramienta ofrece una interfaz flexible de creación de informes y visualización en datos de Marketo Engage, que proporciona detalles granulares sobre progresión, rendimiento, etc. Ofrece una mejor interactividad y visualización, un rendimiento más rápido y una experiencia de usuario más fluida e intuitiva.

Para acceder a esta función, debe haber adquirido el complemento de Analytics de BI avanzado. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

* **Desaprobación del parámetro &#39;access_token&#39; de la API de REST**: El parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API de REST de Marketo está en desuso y no estará disponible después del 31 de octubre de 2025. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API de REST usando el encabezado &quot;Autorización&quot; [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Desaprobación de la API de SOAP**: La compatibilidad con la API de Marketo SOAP finalizará el 31 de octubre de 2025. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API de REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
