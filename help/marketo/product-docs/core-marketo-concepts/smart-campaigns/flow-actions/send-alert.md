---
unique-page-id: 1146958
description: 'Enviar alerta: Documentos de Marketo: documentación del producto'
title: Enviar alerta
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# Enviar alerta {#send-alert}

## Información general {#overview}

Marketo puede enviar una alerta por correo electrónico con información de la persona a cualquier persona: el propietario de ventas, un socio o cualquier otra persona. Utilice el &quot;[!UICONTROL Enviar alerta]Paso de flujo &quot;.

![](assets/one-1.png)

## Uso {#usage}

1. Busque y seleccione el correo electrónico que desea enviar.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >La alerta de correo electrónico debe contener toda la información del encabezado y estar en **[!UICONTROL Aprobado]** estado.

1. Puede hacer clic en el icono de previsualización para asegurarse de que ha seleccionado el correo electrónico correcto.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Asegúrese de utilizar el icono &quot;[!UICONTROL Enviar información de alerta]&quot; token en su correo electrónico.

1. Seleccione el destinatario de la alerta. Puede elegir [!UICONTROL Propietario de ventas] o [!UICONTROL Propietario de cuenta].

   ![](assets/four-2.png)

1. Opcionalmente, agregue cualquier otra dirección de correo electrónico que desee (separada por una coma o un punto y coma).

   ![](assets/five.png)

   >[!TIP]
   >
   >En campañas de déclencheur, puede utilizar tokens en **[!UICONTROL A otros correos electrónicos]** como `{{lead.Territory Owner}}` o `{{my.Alert Recipient}}` siempre que los valores sean direcciones de correo electrónico válidas. Tokens en **[!UICONTROL A otros correos electrónicos]** no funcionará en una campaña por lotes.

>[!MORELIKETHIS]
>
>[Crear un correo electrónico](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
