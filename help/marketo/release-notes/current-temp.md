---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión actual
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 62%

---

# Notas de la versión: enero de 2026 {#release-notes-jan-26}

A continuación encontrará todas las funciones incluidas en la versión de enero de 2026. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

Las notas de la versión específicas de Adobe Dynamic Chat [&#x200B; se encuentran aquí](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 30 de enero de 2026**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado junto a cada función.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Función</th>
   <th style="width:10%">Estado</th>
   <th style="width:25%">Documentación</th>
  </tr>
  <tr>
   <td><strong>TÍTULO DE CARACTERÍSTICA</strong>: Descripción de la característica.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TÍTULO DE CARACTERÍSTICA</strong>: Descripción de la característica.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TÍTULO DE CARACTERÍSTICA</strong>: Descripción de la característica.</td>
   <td><i>Próximamente</i></td>
   <td><i>Próximamente</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Funciones de Adobe Connect {#adobe-connect-features}

La función [Seminarios web interactivos](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"} de Marketo Engage está basada en Adobe Connect, lo que enriquece la administración de personas y las campañas con datos de eventos y mejora la calidad de las personas. A continuación, se muestran algunas versiones recientes de Adobe Connect que afectan directamente a los usuarios de los seminarios web interactivos.

* **Pod de encuestas**: Adobe Connect 12.11 presenta un nuevo Pod de encuestas que permite a los hosts diseñar y entregar formularios de comentarios estructurados directamente dentro de una sesión en vivo.

* **Pod de recursos**: el nuevo Pod de recursos reemplaza a los pods anteriores de archivos y vínculos web, lo que proporciona una forma única y unificada de compartir recursos durante las sesiones activas.

* **Experiencia mejorada de interfaz de sala**: Adobe Connect 12.11 presenta una interfaz de sala actualizada y más moderna, basada en el último marco de diseño Spectrum 2 de Adobe, alineada con el lenguaje visual utilizado en otros productos de Adobe como Creative Cloud y Experience Cloud.

Para obtener información detallada, consulte las [Notas de la versión de Adobe Connect 12.11](https://helpx.adobe.com/es/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}.

## Anuncios {#announcements}

* **Parámetro &#39;access_token&#39; de la API REST obsoleto**: el parámetro de consulta `access_token` utilizado para autenticar las llamadas a la API REST de Marketo está obsoleto y no estará disponible después del miércoles, 31 de marzo de 2026. Todas las integraciones nuevas y existentes deben autenticar las llamadas a la API REST usando el encabezado “Autorización” [tal como se describe aquí](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **API de SOAP obsoleta**: la compatibilidad con la API de Marketo SOAP finalizará el miércoles, 31 de marzo de 2026. Los servicios que usan funcionalidades de la API de SOAP deben migrarse a la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Fin de vida útil de Marketo Engage Identity**:

   * _Restricciones de direcciones IP obsoletas_: la compatibilidad con [Restricción de inicios de sesión de Marketo basados en IP](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. Próximamente estará disponible una nueva función de control de acceso basada en la ubicación para Adobe Identity en Adobe Admin Console.

   * _Inicio de sesión único (SSO) obsoleto_: la compatibilidad con [Marketo Identity SSO](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} finalizó el 30 de julio de 2025. La función permanecerá operativa hasta que se complete la transición a Adobe Identity. El inicio de sesión único para Adobe ID en Adobe Admin Console debe configurarse por separado. Para ver los pasos de configuración, consulte [Configurar la identidad y el inicio de sesión único](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.
