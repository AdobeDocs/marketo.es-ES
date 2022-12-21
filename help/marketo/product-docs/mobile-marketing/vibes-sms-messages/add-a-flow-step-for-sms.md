---
unique-page-id: 11379045
description: 'Añadir un paso de flujo para SMS: Marketo Docs: Documentación del producto'
title: Añadir un paso de flujo para SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Añadir un paso de flujo para SMS {#add-a-flow-step-for-sms}

Marketo tiene tres pasos de flujo que puede utilizar en sus campañas inteligentes de SMS:

* **Enviar mensaje SMS** : esta acción de flujo envía mensajes a las personas de la lista inteligente de Marketo suscritas a una lista de suscripción de Vídeos seleccionada por el usuario. No inicia el proceso de suscripción.
* **Suscripción a la lista de vídeos** - Esta acción de flujo inicia el proceso de suscripción a SMS a través de una campaña de adquisición de vibraciones seleccionada por el usuario. Vibes envía un mensaje de confirmación; el destinatario debe responder para completar el proceso de suscripción.
* **Cancelación de la suscripción a la lista de vídeos** - Esta acción de flujo cancela la suscripción de cada persona a una lista de suscripción de Vídeos seleccionada por el usuario.

>[!NOTE]
>
>Al enviar mensajes SMS:
>
>* Marketo desduplica por número de teléfono. Así que si varias personas tienen el mismo número de teléfono, solo una persona recibirá el mensaje.
>* Marketo no se enviará a las personas incluidas en la lista de bloqueados o con la opción Marketing suspendido.


Para obtener información general sobre la configuración de pasos de flujo, consulte [Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Estos son los conceptos básicos para usar SMS.

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Busque la campaña inteligente a la que desee agregar el flujo de SMS. Haga clic en el **Flujo** pestaña .

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Arrastre el cursor sobre el flujo, por ejemplo, **Enviar mensaje SMS**. Seleccione el mensaje SMS y la lista Vídeos en los menús desplegables.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >El selector Lista de vibraciones actúa como un filtro adicional para la audiencia ya identificada en la lista inteligente para segmentar solo aquellos posibles clientes que pertenezcan a dicha lista.
   >
   >La variable **Suscripción a la lista de vídeos** y **Cancelación de la suscripción a la lista de vídeos** Los flujos tienen requisitos diferentes. Para **Suscribirse**, debe seleccionar la lista Vídeos y la campaña de adquisición de Vídeos . Para **Cancelar suscripción**, solo se requiere la lista Vídeos .
