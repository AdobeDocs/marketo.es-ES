---
unique-page-id: 11379045
description: Añadir un paso de flujo para SMS - Documentos de marketing - Documentación del producto
title: Añadir un paso de flujo para SMS
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Añadir un paso de flujo para SMS {#add-a-flow-step-for-sms}

Marketo tiene tres pasos de flujo que puede utilizar en sus campañas inteligentes de SMS:

* **Enviar mensaje** SMS: Esta acción de flujo envía mensajes a las personas de la lista inteligente de Marketing suscritas a una lista de suscripción de vibraciones seleccionada por el usuario. No inicia el proceso de suscripción.
* **Suscribirse a la Lista** de Vibes: esta acción de flujo inicia el proceso de suscripción de SMS a través de una Campaña de adquisición de vibraciones seleccionada por el usuario. Vibes envía entonces un mensaje de confirmación; el destinatario debe responder a él para completar el proceso de suscripción.
* **Cancelar la suscripción de la Lista** de vibraciones: esta acción de flujo anula la suscripción de cada persona de una lista de suscripción de vibraciones seleccionada por el usuario.

>[!NOTE]
>
>Al enviar mensajes SMS:
>
>* Comercializar las duplicaciones por número de teléfono. Si varias personas tienen el mismo número de teléfono, solo una persona recibirá el mensaje.
>* Marketo no se enviará a personas incluidas en la lista de bloqueados o con suspensiones de marketing.

>



Para obtener información general sobre la configuración de los pasos de flujo, consulte [Añadir un paso de flujo en una Campaña](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)inteligente.

Aquí están los conceptos básicos para usar SMS.

1. En Mi marketing, haga clic en Actividades **de marketing**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Encuentra la campaña inteligente a la que quieres agregar el flujo de SMS. Haga clic en la ficha **Flujo** .

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Arrastre el ratón sobre el flujo, por ejemplo, **Enviar mensaje** SMS. Seleccione el mensaje SMS y la lista Vibes en las listas desplegables.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >El selector de Lista de Vibes actúa como un filtro adicional a la audiencia ya identificada en la lista inteligente para destinatario solo aquellos leads que pertenecen a esa lista de Vibes.
   >
   >
   >La **suscripción a la Lista** de Vibes y la **cancelación de la suscripción a los flujos de Lista** de Vibes tienen requisitos diferentes. En **Suscribirse**, debe seleccionar la lista de vibraciones y la campaña de adquisición de vibraciones. Para **cancelar la suscripción**, solo se requiere la lista Vibes.

