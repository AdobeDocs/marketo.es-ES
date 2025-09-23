---
description: 'Adición de un paso de flujo para SMS: documentos de Marketo, documentación del producto'
title: Añadir un paso de flujo para SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---

# Añadir un paso de flujo para SMS {#add-a-flow-step-for-sms}

Marketo Engage tiene tres pasos de flujo que puede utilizar en sus campañas inteligentes de SMS:

<table>
<tbody>
  <tr>
    <td style="width:25%">Enviar mensaje SMS</td>
    <td>Esta acción de flujo envía mensajes a las personas de la lista inteligente de Marketo suscritas a una lista de suscripción de Vibes seleccionada por el usuario. No inicia el proceso de suscripción. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">Más información</a>.</td>
  </tr>

<tr>
    <td style="width:25%">Suscribirse a la lista de Vibes</td>
    <td>Esta acción de flujo inicia el proceso de suscripción de SMS mediante una campaña de adquisición de vibraciones seleccionada por el usuario. A continuación, Vibes envía un mensaje de confirmación y el destinatario debe responder con "Y" en un plazo de 24 horas para confirmar la inclusión. Una vez que el usuario se haya suscrito, pasará a ser miembro de su lista de suscripción de Vibes asociada.</td>
  </tr>
  <tr>
    <td style="width:25%">Cancelar suscripción a la lista de Vibes</td>
    <td>Esta acción de flujo cancela la suscripción de cada persona a una lista de suscripción de Vibes seleccionada por el usuario. Cuando un usuario envía un mensaje de texto "STOP" a su código, el registro de persona se actualiza para reflejar que ya no es miembro de la lista de suscripción a Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Al enviar mensajes SMS:
>
>* Desduplicaciones de Marketo por número de teléfono. Por lo tanto, si varias personas tienen el mismo número de teléfono, solo una persona recibirá el mensaje si son miembros de una sola lista de suscripción a Vibes. La desduplicación se realiza en el nivel de lista de suscripción de Vibes, no en el nivel de programa de Marketo.
>* Marketo no envía mensajes a personas incluidas en la lista de bloqueados o con Marketing suspendido.

Para obtener información general sobre la configuración de pasos de flujo, consulte [Agregar un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Estos son los conceptos básicos para utilizar SMS.

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Busque y seleccione la campaña inteligente a la que desee añadir el flujo de SMS.

   CAPTURA DE PANTALLA

1. En la pestaña Lista inteligente, elija los déclencheur que desee (por ejemplo, &quot;Formulario rellenado&quot;).

   CAPTURA DE PANTALLA

1. En la pestaña **Flujo**, arrastre el cursor sobre el paso de flujo (por ejemplo, **Enviar mensaje SMS**). Seleccione el mensaje SMS y la lista Vibes de los desplegables.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >El selector Lista de vibraciones actúa como un filtro adicional para la audiencia que ya está identificada en la lista inteligente y se dirige únicamente a los posibles clientes que pertenecen a esa lista de vibraciones.
   >
   >Los flujos **Suscribirse a la lista de vibraciones** y **Cancelar la suscripción a la lista de vibraciones** tienen requisitos diferentes. Para **Suscribirse**, debe seleccionar la lista Vibes y la campaña de adquisición Vibes. Para **Cancelar la suscripción**, solo se requiere la lista de vibraciones.
