---
unique-page-id: 10097199
description: Notas de la versión - Winter '16 - Marketo Docs - Documentación del producto
title: Notas de la versión - Invierno '16
translation-type: tm+mt
source-git-commit: 029d8b419ba5078980b4fde9890bdb35194bf264
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---


# Notas de la versión: Invierno &#39;16 {#release-notes-winter}

Las siguientes funciones se incluyen en la versión 16 de invierno. Haga clic en los vínculos de título para vista de artículos detallados para cada función.

## [Es un filtro anónimo](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

El filtro Es anónimo se ha eliminado para Listas inteligentes. Consulte el documento [Next Generation Munchkin Tracking FAQ](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) para obtener más detalles. Este cambio no afecta a la Personalización web (RTP), que continúa identificando visitantes web anónimos y conocidos y personalizando contenido en tiempo real para estos visitantes.

## [Panel de base de datos](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md)  {#database-dashboard}

La base de datos de posibles clientes tiene un Panel de resumen actualizado que incluye el tamaño total de la base de datos de personas, el número de posibles clientes comercializables y un desglose de posibles clientes por los cinco principales orígenes.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Microsoft Edge Browser](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Hemos agregado Microsoft Edge a la [lista de exploradores](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) admitida por Marketing.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[Ahora ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) se admite Microsoft Outlook 2016.

## [Inicio de encabezado de Programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Utilice el Inicio de encabezado para indicar que el procesamiento del envío debe realizarse con antelación. En lugar de calificar los leads y preparar correos electrónicos a la hora programada del programa, el Inicio de cabezales garantiza que estas tareas se realicen de antemano. De este modo, su audiencia recibirá inicios para recibir correos electrónicos a la hora programada.

![](assets/image2016-1-11-15-3a38-3a3.png)

Para utilizar esta función, el programa de correo electrónico debe programarse con al menos 12 horas de anticipación y la Lista inteligente se bloqueará 12 horas antes del envío.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Esta función se lanzará gradualmente durante una semana después de la versión 16 de invierno. No está disponible para su uso con campañas inteligentes o con la API.

## [Mejoras en la mercadotecnia móvil](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**Compatibilidad con PhoneGap: ahora** se oferta la compatibilidad con PhoneGap para su aplicación móvil. [Más información](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**Compatibilidad con las aplicaciones** de Simulador para pruebas:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [API de programa](https://developers.marketo.com/documentation/programs/) {#program-api}

Crear, actualizar y clonar programas mediante la API de REST. Esto no incluye la creación o actualización de listas inteligentes y campañas inteligentes dentro de un programa.

## [Mejoras de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[Estado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)** de sincronización: Mantenga las fichas sobre el rendimiento actual y el trabajo pendiente del proceso de sincronización. Desglose por número de inserciones y actualizaciones por objeto.

![](assets/pending-backog-cropped.png)

**[Notificaciones](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**: Reciba notificaciones de errores comunes de sincronización, junto con una lista de posibles clientes que tengan ese error.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Mejoras en los objetos personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

Ahora puede crear relaciones de varios a varios entre posibles clientes y cuentas y un objeto personalizado mediante un objeto intermedio con varios campos de vínculo.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Publicidades de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[Los líderes de Facebook ](https://www.facebook.com/business/a/lead-ads) admiten una manera más directa de que un negocio dirija campañas de generación de posibles clientes en Facebook. Las personas rellenan un formulario para expresar interés en un producto o servicio, de modo que la empresa pueda seguir su ejemplo. La integración de Marketing to con Publicidades de posibles clientes de Facebook captura automáticamente la información que proporciona un posible cliente en el formulario de publicidad de posibles clientes. Las acciones de seguimiento y las notificaciones se pueden automatizar mediante el nuevo déclencheur de posibles clientes de Facebook de relleno.

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Planificador de Campaña Web (personalización en tiempo real)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Programe su campaña con antelación. Configure un inicio y una fecha de finalización para el contenido web personalizado y repita campañas en días y horas específicos. Personalice la programación para mostrar la campaña según la hora del visitante web o una zona horaria seleccionada.

![](assets/image2016-1-14-8-3a36-3a36.png)
