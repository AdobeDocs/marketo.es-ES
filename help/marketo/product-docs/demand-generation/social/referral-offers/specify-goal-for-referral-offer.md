---
unique-page-id: 2359791
description: 'Especificar el objetivo de la oferta de reenvío: documentos de Marketo, documentación del producto'
title: Especificar objetivo para oferta de referencia
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# Especificar objetivo para oferta de referencia {#specify-goal-for-referral-offer}

Cuando [crea una oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), necesita definir el objetivo de cumplimiento. El objetivo puede definirse por la actividad de la persona en la página web, como las visitas a la página o los registros. Incluso puedes usar un [evento personalizado de JavaScript](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

>[!IMPORTANT]
>
>El 31 de julio de 2024, empezamos el proceso de dejar de utilizar esta función. Ya no se pueden crear nuevos recursos. Los recursos existentes seguirán funcionando hasta el 31 de enero de 2025. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

También puede utilizar un déclencheur de lista inteligente en Marketo Engage para esperar a que se produzca cualquier hito, como una oportunidad que se esté creando para la persona a la que se hace referencia.

Ejemplo de metas:

* 10 visitas conducidas
* 5 registros referidos
* 1 oportunidad referida creada
* 2 compras de comercio electrónico referidas
* 5 asistentes al seminario web recomendados

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione la oferta de referencia y haga clic en **Editar borrador**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. En el editor de ofertas de reenvío, ve a **Configuración de la aplicación** > **Detalles de la oferta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. En **Configuración**, elija un tipo de evento en la lista desplegable **Objetivo de cumplimiento**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si planea usar el paso de flujo **Dar crédito al referente**, debe seleccionar **Déclencheur de listas inteligentes** como tipo de objetivo de cumplimiento aquí.

* Visitas conducidas: Los participantes en la oferta obtienen crédito por cada visita de un amigo a la página que aloja la oferta.
* Suscripciones preferidas: los participantes en la oferta obtienen crédito por cada amigo que se suscriba a la oferta.
* Déclencheur de listas inteligentes: Los participantes de una oferta obtienen crédito por cada amigo que cumpla las condiciones de un déclencheur de [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) en una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Por ejemplo, puede utilizar un déclencheur que se active cuando un cliente potencial remitido se inscriba en un seminario web.

* Evento de JavaScript personalizado: Los participantes de la oferta obtienen crédito por cada amigo que déclencheur un evento de JavaScript definido en su página. Consulte [Script de conversión para eventos personalizados](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Hay nuevos filtros y déclencheur disponibles en las campañas inteligentes para monitorizar la actividad social. Ver [usar déclencheur y filtros para actividades sociales](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>A continuación, puede [seleccionar los correos electrónicos de registro y cumplimiento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) que desea enviar desde su oferta de referencia.
