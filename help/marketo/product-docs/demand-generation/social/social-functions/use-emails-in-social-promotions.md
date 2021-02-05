---
unique-page-id: 2359793
description: Usar correos electrónicos en promociones sociales - Documentos de marketing - Documentación del producto
title: Usar correos electrónicos en promociones sociales
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# Usar correos electrónicos en promociones sociales {#use-emails-in-social-promotions}

Al crear una [oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) o una [apuesta](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puede incluir correos electrónicos para enviar cuando la persona se registre y nuevamente cuando la persona haya ganado la recompensa.

>[!TIP]
>
>Para crear un mensaje de correo electrónico, consulte [Enviar una prueba de correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md).

En los correos electrónicos, utilice estos tokens:

* **Correo electrónico** de registro: Utilícelo  **`{{social.Share Url}}`** para enviar a cada persona participante un vínculo compartido personalizado.

* **Correo electrónico** de descarga: Utilícelo  **`{{social.Promo Code}}`** para enviar un código [ de ](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)promoción a cada ganador.

>[!PREREQUISITES]
>
>Para poder agregar un correo electrónico a una aplicación social, debe estar _operativo_ y _aprobado_. Consulte [Editar configuración para un correo electrónico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione la aplicación y haga clic en **Editar borrador**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. En el editor de la aplicación social, vaya a **Configuración de la aplicación > Detalles de la Oferta** (o **Detalles de las apuestas**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Añada el correo electrónico de registro.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >El correo electrónico de confirmación se envía automáticamente cuando una persona se registra.

1. Añada el correo electrónico de despacho.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. En una oferta de referencia, elija si el correo electrónico de despacho se envía de forma automática o manual.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>En una apuesta, el correo electrónico de despacho siempre se envía automáticamente cuando [selecciona al ganador](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definición**
>
>* **objetivo** automático: El correo electrónico de cumplimiento se envía automáticamente a medida que cada participante cumple el objetivo.
>* **enviar** manualmente: Una vez que las personas tengan inicios para cumplir el objetivo, vuelva a la oferta de referencia para  [enviar manualmente el correo electrónico](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) de cumplimiento.

>



>[!MORELIKETHIS]
>
>A continuación, puede [elegir la dirección URL de uso compartido](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) o, en su oferta de referencia, puede [cargar los códigos de promoción](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) que enviará.
