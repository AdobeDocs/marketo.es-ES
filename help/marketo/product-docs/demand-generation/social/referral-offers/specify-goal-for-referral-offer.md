---
unique-page-id: 2359791
description: 'Especificar el objetivo de la oferta de reenvío: documentos de Marketo, documentación del producto'
title: Especificar objetivo para oferta de referencia
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Especificar objetivo para oferta de referencia {#specify-goal-for-referral-offer}

Cuando usted [crear una oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), debe definir el objetivo de cumplimiento. El objetivo puede definirse por la actividad de la persona en la página web, como las visitas a la página o los registros. Incluso puede utilizar un [evento de JavaScript personalizado](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

También puede utilizar un déclencheur de lista inteligente en Marketo para esperar a que se produzca cualquier hito, como una oportunidad que se esté creando para la persona a la que se hace referencia.

Ejemplo de metas:

* 10 visitas conducidas
* 5 registros referidos
* 1 oportunidad referida creada
* 2 compras de comercio electrónico referidas
* 5 asistentes al seminario web recomendados

1. Ir a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione la oferta de referencia y haga clic en **Editar borrador**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. En el editor de ofertas de recomendación, vaya a **Configuración de aplicación** > **Detalles de oferta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. En **Configuración**, elija un tipo de evento de la **Objetivo de cumplimiento** menú desplegable.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si planea utilizar el **Dar crédito al referente** paso de flujo, debe seleccionar **Déclencheur de listas inteligentes** como el tipo de objetivo de cumplimiento aquí.

* Visitas conducidas: Los participantes en la oferta obtienen crédito por cada visita de un amigo a la página que aloja la oferta.
* Suscripciones preferidas: los participantes en la oferta obtienen crédito por cada amigo que se suscriba a la oferta.
* Déclencheur de listas inteligentes: Los participantes de una oferta obtienen crédito por cada amigo que cumpla las condiciones de un [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) déclencheur en una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Por ejemplo, puede utilizar un déclencheur que se active cuando un cliente potencial remitido se inscriba en un seminario web.

* Evento de JavaScript personalizado: Los participantes de la oferta obtienen crédito por cada amigo que déclencheur un evento de JavaScript definido en su página. Consulte [Script de conversión para eventos personalizados](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Hay nuevos filtros y déclencheur disponibles en las campañas inteligentes para monitorizar la actividad social. Consulte [usar déclencheur y filtros para actividades sociales](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>A continuación, puede [seleccione los correos electrónicos de registro y cumplimiento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) para enviar desde su oferta de referencia.
