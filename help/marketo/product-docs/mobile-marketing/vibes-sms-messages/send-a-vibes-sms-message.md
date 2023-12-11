---
description: 'Enviar un mensaje SMS de Vibes: documentos de Marketo: documentación del producto'
title: Enviar un mensaje SMS de Vibes
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: d4bd94b22b4f9da993150a94d2757014cbf87d80
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Enviar un mensaje SMS de Vibes {#send-a-vibes-sms-message}

Ha... [creó su mensaje SMS de Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), ahora es el momento de enviarlo. Puede enviarlo por lotes o mediante la campaña de Déclencheur.

>[!NOTE]
>
>Al enviar mensajes SMS:
>
>* Desduplicaciones del Marketo Engage por número de teléfono. Por lo tanto, si varias personas tienen el mismo número de teléfono, solo una persona recibirá el mensaje si son miembros de una sola lista de suscripción a Vibes. La desduplicación se realiza en el nivel de lista de suscripción de Vibes, no en el nivel de programa de Marketo.
>* Marketo no envía mensajes a personas incluidas en la lista de bloqueados o con Marketing suspendido.

## Envío de un SMS por lotes {#send-a-batch-sms}

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/send-a-vibes-sms-message-1.png)

1. Busque y seleccione la campaña inteligente que desee.

   ![](assets/send-a-vibes-sms-message-2.png)

1. Haga clic en **Lista inteligente** y defina la audiencia del SMS. En este ejemplo, enviamos a todos los usuarios de nuestra base de datos que tengan &quot;Adobe&quot; enumerado como su compañía.

   ![](assets/send-a-vibes-sms-message-3.png)

1. En el **Flujo** pestaña, arrastrar **Enviar mensaje SMS**. Seleccione la lista SMS Message and Vibes que desee en los desplegables.

   ![](assets/send-a-vibes-sms-message-4.png)

   >[!NOTE]
   >
   >El selector Lista de vibraciones actúa como un filtro adicional para la audiencia ya identificada en la Lista inteligente y se dirige únicamente a las personas que pertenecen a esa lista de vibraciones.

1. Haga clic en **Programación** y programe su SMS.

   ![](assets/send-a-vibes-sms-message-5.png)

## Envío de un SMS de Déclencheur {#send-a-trigger-sms}

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/send-a-vibes-sms-message-6.png)

1. Busque y seleccione la campaña inteligente que desee.

   ![](assets/send-a-vibes-sms-message-7.png)

1. Haga clic en **Lista inteligente** , seleccione el déclencheur deseado y defina su valor. En este ejemplo, se utiliza **Rellena el formulario**.

   ![](assets/send-a-vibes-sms-message-8.png)

1. En el **Flujo** pestaña, arrastrar **Enviar mensaje SMS**. Seleccione la lista SMS Message and Vibes que desee en los desplegables.

   ![](assets/send-a-vibes-sms-message-9.png)

   >[!NOTE]
   >
   >El selector Lista de vibraciones actúa como un filtro adicional para la audiencia ya identificada en la Lista inteligente y se dirige únicamente a las personas que pertenecen a esa lista de vibraciones.

1. Haga clic en **Programación** pestaña, luego **Activar**.

   ![](assets/send-a-vibes-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Crear un mensaje de vibraciones](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)
>* Pasos de flujo de vibraciones

