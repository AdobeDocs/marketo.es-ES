---
description: 'Notas de la versión, mayo de 2025: Documentos de Marketo: documentación del producto'
title: Notas de la versión, mayo de 2025
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 40%

---

# Notas de la versión: mayo de 2025 {#release-notes-may-25}

A continuación encontrará todas las funciones incluidas en la versión de mayo de 2025. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 23 de mayo de 2025**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>Control de acceso basado en roles para Designer Assets de correo electrónico</strong>: una nueva mejora del sistema de control de acceso basado en roles (RBAC) proporciona permisos más granulares y una administración de usuarios mejorada para los recursos con tecnología del nuevo Designer de correo electrónico.</td>
   <td>Enviado</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">Permisos granulares para New Email Designer (publicación de blog)</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Clonación de correos electrónicos creados en el Designer de correo electrónico</strong>: ahora puede clonar un correo electrónico existente creado con el nuevo Designer de correo electrónico.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Tokens de Déclencheur para cualquier atributo</strong>: Se ha ampliado la lista de tokens de déclencheur para admitir el uso de datos de cualquier atributo de actividad en los campos de Smart Campaign.</td>
   <td>Enviado</td>
   <td>N/A</td>
  </tr>
 </tbody>
</table>
<br/>

## Anuncios {#announcements}

* **Actualización de la integración de la conversión sin conexión de Facebook**: el 29 de mayo de 2025, la integración de [Conversión sin conexión de Facebook](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"} para Marketo Engage se migrará a la nueva API de [conversiones sin conexión de Meta](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}, debido a que Meta dejó de utilizar la [API de conversiones sin conexión](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} en línea con el control de versiones de la API de gráficos. Para obtener más información, consulte la guía de Meta para [enviar eventos sin conexión a través de la API de conversiones](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI para sin conexión).

* **Nueva característica de Analytics - Beta público**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anteriormente conocido como Revenue Explorer y Advanced Report Builder) comenzó a implementarse para todos los usuarios actuales del Revenue Cycle Explorer a mediados de abril. Esta nueva herramienta ofrece una interfaz flexible de creación de informes y visualización en datos de Marketo Engage, que proporciona detalles granulares sobre progresión, rendimiento, etc. Ofrece una mejor interactividad y visualización, un rendimiento más rápido y una experiencia de usuario más fluida e intuitiva.

Para acceder a esta función, debe haber adquirido el complemento de Analytics de BI avanzado. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del miércoles, 31 de marzo de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el miércoles, 31 de marzo de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
