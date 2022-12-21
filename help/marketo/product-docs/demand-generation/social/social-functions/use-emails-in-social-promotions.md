---
unique-page-id: 2359793
description: Usar correos electrónicos en promociones sociales - Documentos de Marketo - Documentación del producto
title: Usar correos electrónicos en promociones sociales
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Usar correos electrónicos en promociones sociales {#use-emails-in-social-promotions}

Al crear un [oferta de recomendación](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) o [apuestas](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puede incluir correos electrónicos que se enviarán cuando la persona se registre y, de nuevo, cuando la persona haya ganado la recompensa.

>[!TIP]
>
>Para crear un correo electrónico, consulte [Enviar una explosión de correo electrónico](/help/marketo/getting-started/quick-wins/send-an-email.md).

En los correos electrónicos, utilice estos tokens:

* **Correo electrónico de registro**: Uso **`{{social.Share Url}}`** para enviar a cada persona participante un vínculo compartido personalizado.

* **Correo electrónico de cumplimiento**: Uso **`{{social.Promo Code}}`** para enviar a cada ganador un [código promocional](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Para poder añadir un correo electrónico a una aplicación social, debe ser _operativa_ y _aprobado_. Consulte [Editar configuración de un correo electrónico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione la aplicación y haga clic en **Editar borrador**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. En el editor de aplicaciones sociales, vaya a **Configuración de la aplicación > Detalles de la oferta** (o **Detalles de apuestas**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Añada el correo electrónico de registro.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >El correo electrónico de confirmación se envía automáticamente cuando una persona se registra.

1. Añada el correo electrónico de cumplimiento.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. En una oferta de referente, elija si el correo electrónico de cumplimiento se envía de forma automática o manual.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>En una apuesta, el correo electrónico de cumplimiento siempre se envía automáticamente cuando [seleccione el ganador](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definición**
>
>* **segmentación automática**: El correo electrónico de cumplimiento se envía automáticamente cuando cada participante cumple el objetivo.
>* **envío manual**: Una vez que las personas empiecen a alcanzar el objetivo, vuelva a la oferta de referencia a [enviar el correo electrónico de cumplimiento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>


>[!MORELIKETHIS]
>
>A continuación, puede [elija la URL del recurso compartido](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) o, en su oferta de referente, puede [cargar los códigos de promoción](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) enviarás.
