---
unique-page-id: 2359791
description: 'Especificar objetivo para la oferta de reenvío: Documentos de Marketo: Documentación del producto'
title: Especificar objetivo para la oferta de reenvío
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Especificar objetivo para la oferta de reenvío {#specify-goal-for-referral-offer}

Cuando [crear una oferta de referente](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), debe definir el objetivo de cumplimiento. El objetivo se puede definir por actividad de persona en la página web, como visitas de página o registros. Incluso puede usar un [evento personalizado de JavaScript](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Como alternativa, puede utilizar un déclencheur de lista inteligente en Marketo para esperar cualquier hito, como una oportunidad que se esté creando para la persona referida.

Objetivos de ejemplo:

* 10 visitas remitidas
* 5 registros remitidos
* 1 oportunidad de referencia creada
* 2 compras de comercio electrónico referidas
* 5 asistentes de seminarios web remitidos

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione la oferta de referente y haga clic en **Editar borrador**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. En el editor de ofertas de referente, vaya a **Configuración de la aplicación** > **Detalles de la oferta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. En **Configuración**, elija un tipo de evento en la **Objetivo de cumplimiento** lista desplegable.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si planea usar la variable **Dar crédito al referente** paso de flujo, debe seleccionar **Déclencheur de lista inteligente** como tipo de objetivo de cumplimiento aquí.

* Visitas referidas: Los participantes en la oferta obtienen crédito por cada visita de un amigo a la página que aloja la oferta.
* Firmas remitidas: Los participantes de la oferta obtienen crédito por cada amigo que se inscribe en la oferta.
* Déclencheur de lista inteligente: Los participantes en la oferta obtienen crédito por cada amigo que cumpla las condiciones de un [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) déclencheur en un [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Por ejemplo, puede utilizar un déclencheur que se active cuando un cliente potencial remitido se registre en un seminario web.

* Evento de JavaScript personalizado: Los participantes en la oferta obtienen crédito por cada amigo que déclencheur un evento JavaScript definido en la página. Consulte [Script de conversión para eventos personalizados](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Hay nuevos filtros y déclencheur disponibles en las campañas inteligentes para supervisar la actividad social. Consulte [usar déclencheur y filtros para actividades sociales](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>A continuación, puede [seleccione los correos electrónicos de registro y cumplimiento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) para enviar desde la oferta de referente.
