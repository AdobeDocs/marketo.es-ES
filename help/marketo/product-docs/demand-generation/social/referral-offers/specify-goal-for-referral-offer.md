---
unique-page-id: 2359791
description: Especificar objetivo para la Oferta de referencia - Documentos de marketing - Documentación del producto
title: Especificar objetivo para la Oferta de referencia
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Especificar objetivo para la Oferta de referencia {#specify-goal-for-referral-offer}

Cuando [crea una oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), debe definir el objetivo de cumplimiento. El objetivo se puede definir por actividad de persona en la página web, como visitas a la página o suscripciones. Incluso puede utilizar un [evento personalizado de JavaScript](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Como alternativa, puede utilizar un déclencheur de lista inteligente en Marketing para esperar cualquier hito, como una oportunidad que se esté creando para la persona a la que se hace referencia.

Objetivos de ejemplo:

* 10 visitas remitidas
* 5 suscripciones remitidas
* 1 oportunidad referida creada
* 2 compras de comercio electrónico referidas
* 5 asistentes de seminario web referidos

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione la oferta de referencia y haga clic en **Editar borrador**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. En el editor de ofertas de referencia, vaya a **Configuración de la aplicación** > **Detalles de la Oferta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. En **Configuración**, elija un tipo de evento en la lista desplegable **Objetivo de cumplimiento**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si planea utilizar el paso de flujo **Dar crédito a Remitente del reenvío**, debe seleccionar **Déclencheur de Lista inteligente** como tipo de objetivo de cumplimiento aquí.

* Visitas referidas: Los participantes de la oferta obtienen crédito por cada visita de un amigo a la página que aloja su oferta.
* Firmas Referidas: Los participantes de la oferta reciben crédito por cada amigo que se inscribe en la oferta.
* Déclencheur de Lista inteligente: Los participantes de la oferta obtienen crédito por cada amigo que cumple las condiciones de un déclencheur [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) en una [campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Por ejemplo, puede utilizar un déclencheur que se active cuando un cliente potencial referido se registre en un seminario web.

* Evento personalizado de JavaScript: Los participantes de la oferta obtienen crédito por cada amigo que déclencheur un evento JavaScript definido en la página. Consulte [Secuencia de comandos de conversión para Eventos personalizados](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Hay nuevos filtros y déclencheur disponibles en campañas inteligentes para supervisar la actividad social. Consulte [usar déclencheur y filtros para actividades sociales](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>A continuación, puede [seleccionar los mensajes de correo electrónico de registro y cumplimiento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) para enviarlos desde la oferta de referencia.
