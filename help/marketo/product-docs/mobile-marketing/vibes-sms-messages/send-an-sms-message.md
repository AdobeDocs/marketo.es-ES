---
description: 'Envío de un mensaje SMS: documentos de Marketo, documentación del producto'
title: Enviar un mensaje SMS
feature: Mobile Marketing
exl-id: 2c863ded-f441-4217-9541-6dcc442d9831
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 2%

---

# Enviar un mensaje SMS {#send-a-vibes-sms-message}

Has [creado tu mensaje SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, ahora es el momento de enviarlo. Puede enviarlo por lotes o mediante la campaña de Déclencheur.

>[!NOTE]
>
>Al enviar mensajes SMS:
>
>* Desduplicaciones de Marketo Engage por número de teléfono. Por lo tanto, si varias personas tienen el mismo número de teléfono, solo una persona recibirá el mensaje si son miembros de una sola lista de suscripción a Vibes. La desduplicación se realiza en el nivel de lista de suscripción de Vibes, no en el nivel de programa de Marketo.
>* Marketo no envía mensajes a personas incluidas en la lista de bloqueados o con Marketing suspendido.
>* Un mensaje SMS no se enviará a nadie que haya cancelado la suscripción si no está en la lista de la base de datos móvil de Vibes.

## Envío de un SMS por lotes {#send-a-batch-sms}

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/send-an-sms-message-1.png)

1. Busque y seleccione la campaña inteligente que desee.

   ![](assets/send-an-sms-message-2.png)

1. Haga clic en la ficha **Lista inteligente** y defina la audiencia para el SMS. En este ejemplo, enviamos a todos los usuarios de nuestra base de datos que tengan &quot;Adobe&quot; enumerado como su empresa.

   ![](assets/send-an-sms-message-3.png)

1. En la pestaña **Flujo**, arrastre el cursor sobre **Enviar mensaje SMS**. Seleccione la lista SMS Message and Vibes que desee en los desplegables.

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >El selector Lista de vibraciones actúa como un filtro adicional para la audiencia ya identificada en la Lista inteligente y se dirige únicamente a las personas que pertenecen a esa lista de vibraciones.

1. Haz clic en la pestaña **Programar** y programa tu SMS.

   ![](assets/send-an-sms-message-5.png)

## Envío de un SMS de Déclencheur {#send-a-trigger-sms}

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/send-an-sms-message-6.png)

1. Busque y seleccione la campaña inteligente que desee.

   ![](assets/send-an-sms-message-7.png)

1. Haga clic en la ficha **Lista inteligente**, seleccione el déclencheur deseado y defina su valor. En este ejemplo, se usa **Rellena el formulario**.

   ![](assets/send-an-sms-message-8.png)

1. En la pestaña **Flujo**, arrastre el cursor sobre **Enviar mensaje SMS**. Seleccione la lista SMS Message and Vibes que desee en los desplegables.

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >El selector Lista de vibraciones actúa como un filtro adicional para la audiencia ya identificada en la Lista inteligente y se dirige únicamente a las personas que pertenecen a esa lista de vibraciones.

1. Haga clic en la ficha **Programar** y luego en **Activar**.

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Crear un mensaje de vibraciones](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}
>* [Uso de opciones de SMS en una campaña inteligente](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
