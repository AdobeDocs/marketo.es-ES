---
unique-page-id: 2359793
description: 'Uso de correos electrónicos en promociones sociales: documentos de Marketo, documentación del producto'
title: Uso de correos electrónicos en promociones sociales
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Uso de correos electrónicos en promociones sociales {#use-emails-in-social-promotions}

Al crear un [oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) o una [sorteo](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puede incluir correos electrónicos para enviar cuando la persona se inscriba y otra vez cuando la persona haya ganado la recompensa.

>[!TIP]
>
>Para crear un correo electrónico, consulte [Enviar una explosión por correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md).

En los correos electrónicos, utilice estos tokens:

* **Correo electrónico de registro**: uso **`{{social.Share Url}}`** para enviar a cada persona participante un vínculo compartido personalizado.

* **Correo electrónico de cumplimiento**: uso **`{{social.Promo Code}}`** para enviar a cada ganador un [código de promoción](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Para poder añadir un correo electrónico a una aplicación social, debe ser _operativo_ y _aprobado_. Consulte [Editar la configuración de un correo electrónico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Ir a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione la aplicación y haga clic en **Editar borrador**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. En el editor de aplicaciones sociales, vaya a **Configuración de aplicación > Detalles de oferta** (o **Detalles de sorteo**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Añada el correo electrónico de registro.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >El correo electrónico de confirmación se envía automáticamente cuando una persona se registra.

1. Añada el correo electrónico de cumplimiento.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. En una oferta de recomendación, elija si el correo electrónico de cumplimiento se envía de forma automática o manual.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>En un sorteo, el correo electrónico de cumplimiento siempre se envía automáticamente cuando [seleccionar el ganador](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definición**
>
>* **automático en la meta**: el correo electrónico de cumplimiento se envía automáticamente cuando cada participante cumple el objetivo.
>* **envío manual**: Una vez que las personas empiecen a cumplir el objetivo, vuelva a la oferta de referencia para obtener manualmente [enviar el correo electrónico de cumplimiento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>A continuación, puede [elija la URL compartida](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) o bien, en su oferta de recomendación, puede [cargar los códigos de promoción](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) usted enviará a cabo.
