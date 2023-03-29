---
unique-page-id: 13795395
description: Notas de la versión - Invierno '18 - Marketo Docs - Documentación del producto
title: Notas de la versión - Invierno '18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 1%

---

# Notas de la versión: Invierno &#39;18 {#release-notes-winter}

Las siguientes funciones están incluidas en la versión de invierno de 2018. Compruebe la disponibilidad de las funciones en su edición de Marketo.

Haga clic en los vínculos de título para ver los artículos detallados de cada función. **Nota**: Algunas de las funciones incluidas en esta versión no tienen artículos asociados. Si un tema tiene varios subencabezados, los vínculos se colocan allí.

## Mejoras en el rendimiento y el rendimiento de las campañas {#campaign-performance-and-throughput-enhancements}

Marketo está aprovechando nuestra arquitectura de grandes datos para aumentar el rendimiento de las campañas de déclencheur y mejorar el procesamiento de actividades web, de modo que pueda reaccionar más rápido a las acciones de su audiencia.

## Mejoras en la integración de Salesforce CRM en Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Tenemos dos mejoras en nuestra integración de Salesforce CRM:

* [Notificaciones del administrador de Marketo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) para ciertos errores de sincronización de CRM (credenciales caducadas, límites de API alcanzados, etc.)

* [Posibilidad de desactivar las notificaciones por correo electrónico](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) a Propietarios potenciales al asignar posibles clientes

Estas mejoras se implementarán en 2018.

## [Perspectivas de rendimiento de Marketo](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>Perspectivas de rendimiento es un producto adicional. Póngase en contacto con su administrador de cuentas o ejecutivo de cuentas de Marketo para obtener un presupuesto.

Explore cómo sus campañas y canales afectan a los resultados empresariales con análisis de atribución, visualizaciones interactivas y una tabla de datos detallada.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Mejoras de marketing basadas en cuentas {#account-based-marketing-enhancements}

**[Jerarquías ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Para los clientes ABM con Salesforce o Microsoft Dynamics, ABM heredará (y mostrará) automáticamente las relaciones padre-hijo establecidas en CRM. Podrá utilizar estas relaciones tanto en los informes de resumen como en la ejecución de campañas.

## Marketing por correo electrónico {#email-marketing}

**[Script de correo electrónico dinámico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Ahora, los scripts de Velocity se admiten en correos electrónicos que utilizan contenido dinámico. Combine contenido dinámico basado en la velocidad y la segmentación para crear correos electrónicos altamente personalizados.

**Zona horaria del destinatario**

* **[Catarata mensual](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Hemos agregado la capacidad de programar programas de crianza en una cadencia mensual.

* **[Detener entrega](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Ahora puede detener los envíos restantes a mitad de la ejecución.

## Integraciones de red de publicidad {#ad-network-integrations}

**[Integración de Customer Match de Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Con esta integración, puede enviar una audiencia de Marketo a Google para que sea segmentada mediante Google AdWords, así como redirigir audiencias a través de YouTube, Search y Gmail.

**[Mejora de la API de audiencias coincidentes de linkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Nuestra nueva API de LinkedIn ahora le permite volver a dirigirse a personas de su base de datos de Marketo en varias cuentas de Administrador de LinkedIn Campaign.

## Personalización web {#web-personalization}

**Fuente de datos japonesa para la personalización web**

Marketo está agregando una fuente de datos japonesa adicional para la personalización web a fin de mejorar la identificación de visitantes web (búsqueda IP inversa) y la personalización de los visitantes que llegan de Japón. Los nombres de organización se mostrarán en japonés.

**[Creación de un segmento web mediante listas estáticas](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

La personalización web ahora puede personalizar el contenido para un visitante web conocido que forme parte de una lista estática definida en Actividades de marketing (MLM). Con esta mejora, ahora puede comercializar a listas estáticas entre canales y dirigirse a personas de estas listas con contenido personalizado en el sitio web.

## ContentAI {#contentai}

**Mejora del algoritmo predictivo**

El contenido recomendado mediante los algoritmos de ContentAI optimizados de Marketo genera hasta el doble de clics que el contenido aleatorio.

## Integración de  {#integration}

**[Activar/desactivar la API de Campaign](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Esta nueva API le permite activar y desactivar de forma remota las campañas de déclencheur, por lo que ahora puede crear plantillas de programa totalmente automatizadas. Cree una plantilla de programa una vez, luego automatice la clonación, las actualizaciones de material publicitario de marketing y ahora la activación/programación de campañas inteligentes.

## ToutApp {#toutapp}

**Cancelar suscripción**

A partir del 1 de marzo de 2018, todos los correos electrónicos enviados desde [ToutApp.com](https://ToutApp.com) (y utilizando el botón &quot;Correo electrónico con tout&quot; en Salesforce) tendrá un enlace de cancelación de suscripción anexado a la parte inferior.

**Actualización de la fuente en directo**

Hemos actualizado el aspecto de las pestañas Participación y Tarea para que los miembros de Ventas puedan responder a las actividades de sus clientes directamente desde la fuente activa con mayor facilidad y rapidez.

**Actualización de vista de detalles de personas**

La Vista detallada de personas (PDV) mejorada ofrece una vista completa de sus contactos reuniendo los detalles de contacto de Tout y Salesforce CRM.
