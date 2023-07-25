---
unique-page-id: 1146958
description: 'Enviar alerta: Documentos de Marketo: documentación del producto'
title: Enviar alerta
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 3%

---

# Enviar alerta {#send-alert}

## Información general {#overview}

Marketo puede enviar una alerta por correo electrónico con información de la persona a cualquier persona: el propietario de ventas, un socio o cualquier otra persona. Utilice el **Enviar alerta** paso de flujo.

![](assets/one-1.png)

## Uso {#usage}

1. Busque y seleccione el correo electrónico que desea enviar.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >La alerta de correo electrónico debe contener toda la información del encabezado y estar en **Aprobado** estado.

1. Puede hacer clic en el icono de previsualización para asegurarse de que ha seleccionado el correo electrónico correcto.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Asegúrese de utilizar el **Enviar información de alerta** token en el correo electrónico.

1. Seleccione el destinatario de la alerta. Puede elegir Propietario de ventas o Propietario de cuenta.

   ![](assets/four-2.png)

1. De forma opcional, agregue cualquier otra dirección de correo electrónico que desee (separada por una coma o un punto y coma).

   ![](assets/five.png)

   >[!TIP]
   >
   >En campañas de déclencheur, puede utilizar tokens en **A otros correos electrónicos** como `{{lead.Territory Owner}}` o `{{my.Alert Recipient}}` siempre que los valores sean direcciones de correo electrónico válidas. Tokens en **A otros correos electrónicos** no funcionará en una campaña por lotes.

¡Eso es todo! Ahora ya sabe cómo usar el **Enviar alerta** paso de flujo.

>[!MORELIKETHIS]
>
>[Crear un correo electrónico](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
