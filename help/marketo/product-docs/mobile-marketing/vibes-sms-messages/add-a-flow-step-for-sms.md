---
unique-page-id: 11379045
description: 'Adición de un paso de flujo para SMS: documentos de Marketo, documentación del producto'
title: Añadir un paso de flujo para SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Añadir un paso de flujo para SMS {#add-a-flow-step-for-sms}

Marketo tiene tres pasos de flujo que puede utilizar en sus campañas inteligentes de SMS:

* **Enviar mensaje SMS** : Esta acción de flujo envía mensajes a las personas de la lista inteligente de Marketo suscritas a una lista de suscripción de Vibes seleccionada por el usuario. No inicia el proceso de suscripción.
* **Suscribirse a la lista de vibraciones** : Esta acción de flujo inicia el proceso de suscripción de SMS mediante una campaña de adquisición de vibraciones seleccionada por el usuario. A continuación, Vibes envía un mensaje de confirmación; el destinatario debe responder para completar el proceso de suscripción.
* **Cancelar suscripción a la lista de vibraciones** : Esta acción de flujo cancela la suscripción de cada persona a una lista de suscripción de Vibes seleccionada por el usuario.

>[!NOTE]
>
>Al enviar mensajes SMS:
>
>* Desduplicaciones de Marketo por número de teléfono. Por lo tanto, si varias personas tienen el mismo número de teléfono, solo una persona recibirá el mensaje.
>* Marketo no envía mensajes a personas incluidas en la lista de bloqueados o con Marketing suspendido.

Para obtener información general sobre la configuración de los pasos de flujo, consulte [Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Estos son los conceptos básicos para utilizar SMS.

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Busque la campaña inteligente a la que desee añadir el flujo SMS. Haga clic en **Flujo** pestaña.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Arrastre sobre el flujo, por ejemplo, **Enviar mensaje SMS**. Seleccione el mensaje SMS y la lista Vibes de los desplegables.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >El selector Lista de vibraciones actúa como un filtro adicional para la audiencia que ya está identificada en la lista inteligente y se dirige únicamente a los posibles clientes que pertenecen a esa lista de vibraciones.
   >
   >El **Suscribirse a la lista de vibraciones** y **Cancelar suscripción a la lista de vibraciones** Los flujos de tienen diferentes requisitos. Para **Suscribirse**, debe seleccionar la lista Vibes y la campaña de adquisición Vibes. Para **Cancelar suscripción**, solo se requiere la lista Vibes.
