---
unique-page-id: 13795395
description: 'Notas de la versión, invierno de 2018, documentación de Marketo: documentación del producto'
title: Notas de la versión, invierno de 2018
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
TQID: https://experienceleague.adobe.com/IBxE-nJhOC4vaFcydzdsr9aAhMmiHuQro57k1SCiwTA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 598
ht-degree: 2%

---

# Notas de la versión: invierno de 2018 {#release-notes-winter}

En la versión de invierno de 18 se incluyen las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition.

Haga clic en los vínculos del título para ver los artículos detallados de cada función. **Nota**: algunas de las características incluidas en esta versión no tienen artículos asociados. Si un tema tiene varios subencabezados, los vínculos se colocan allí.

## Mejoras de rendimiento y rendimiento de Campaign {#campaign-performance-and-throughput-enhancements}

Marketo aprovecha su arquitectura de big data para aumentar el rendimiento de las campañas de déclencheur y mejorar el procesamiento de actividades web, de modo que pueda reaccionar ante las acciones de su audiencia más rápido.

## Mejoras en la integración de CRM [!DNL Salesforce] de Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Tenemos dos mejoras en nuestra integración de CRM [!DNL Salesforce]:

* [Notificaciones del administrador de Marketo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) para ciertos errores de sincronización de CRM (credenciales caducadas, límites de API alcanzados, etc.)

* [Capacidad para desactivar las notificaciones por correo electrónico](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) a los propietarios de posibles clientes tras la asignación de posibles clientes

Estas mejoras se implementarán en 2018.

## [Perspectivas de rendimiento de Marketo](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>[!UICONTROL Perspectivas de rendimiento] es un producto adicional. Póngase en contacto con el administrador de éxitos del cliente o con el ejecutivo de cuentas de Marketo para obtener un presupuesto.

Explore cómo sus campañas y canales impactan en los resultados empresariales con análisis de atribución, visualizaciones interactivas y una tabla de datos detallada.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Mejoras de marketing basado en cuentas {#account-based-marketing-enhancements}

**[Jerarquías ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Para los clientes de ABM con [!DNL Salesforce] o [!DNL Microsoft Dynamics], ABM ahora heredará (y mostrará) automáticamente las relaciones principal-secundario establecidas en CRM. Podrá utilizar estas relaciones tanto en la creación de informes de resumen como en la ejecución de campañas.

## Marketing por correo electrónico {#email-marketing}

**[Script de correo electrónico dinámico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Los scripts de Velocity ahora se admiten en correos electrónicos que utilizan contenido dinámico. Combine contenido dinámico basado en velocidad y segmentación para crear correos electrónicos altamente personalizados.

**Zona horaria del destinatario**

* **[Cadencia de crianza mensual](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Hemos agregado la capacidad de programar programas de crianza en una cadencia mensual.

* **[Detener envío](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Ahora puede detener cualquier envío restante a mitad de la ejecución.

## Integraciones de red de anuncios {#ad-network-integrations}

**[Integración de Google Customer Match](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Con esta integración, puede enviar una audiencia de Marketo a Google para que la use [!DNL Google AdWords], así como volver a segmentar audiencias en [!DNL YouTube], Search y [!DNL Gmail].

**[[!DNL LinkedIn] Mejora de API de audiencias coincidentes](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Nuestra nueva API [!DNL LinkedIn] ahora le permite volver a dirigirse a las personas de su base de datos de Marketo en varias cuentas de [!DNL LinkedIn] Campaign Manager.

## Personalización web {#web-personalization}

**Source de datos en japonés para Web Personalization**

Marketo está agregando una fuente de datos adicional en japonés para Web Personalization a fin de mejorar la identificación de visitantes web (búsqueda inversa de IP) y la personalización para los visitantes que llegan desde Japón. Los nombres de las organizaciones se mostrarán en japonés.

**[Crear un segmento web mediante listas estáticas](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization ahora puede personalizar el contenido a un visitante web conocido que forme parte de una lista estática definida en Actividades de marketing (MLM). Con esta mejora, ahora puede enviar al mercado listas estáticas entre canales y dirigirse a las personas de estas listas con contenido personalizado en el sitio web.

## ContentAI {#contentai}

**Mejora del algoritmo predictivo**

El contenido recomendado mediante los algoritmos de inteligencia artificial aplicada al contenido optimizados de Marketo genera hasta el doble de clics que el contenido aleatorio.

## Integración {#integration}

**[Activar/Desactivar API de Campaign](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Esta nueva API le permite activar y desactivar de forma remota campañas de déclencheur, de modo que ahora puede crear plantillas de programa completamente automatizadas. Cree una plantilla de programa una vez y, a continuación, automatice la clonación, las actualizaciones de material promocional y ahora la activación o programación de campañas inteligentes.

## [!DNL ToutApp] {#toutapp}

**Anular la suscripción a la actualización**

A partir del 1 de marzo de 2018, todos los correos electrónicos enviados desde [ToutApp.com](https://ToutApp.com) (y mediante el botón &quot;Enviar correo electrónico con [!DNL Tout]&quot; en [!DNL Salesforce]) tendrán un vínculo para cancelar la suscripción anexado a la parte inferior.

**Actualización de fuente en directo**

Hemos actualizado el aspecto de las pestañas Participación y Tarea para que sea más fácil y rápido para los miembros de ventas responder a las actividades de sus clientes directamente desde Live Feed.

**Actualización de vista de detalles de personas**

La vista de detalles de personas (PDV) mejorada ofrece una vista completa de sus contactos al reunir sus datos de contacto de [!DNL Tout] y [!DNL Salesforce] CRM.
