---
unique-page-id: 1146958
description: 'Enviar alerta: Documentos de Marketo: documentación del producto'
title: Enviar alerta
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 2%

---

# Enviar alerta {#send-alert}

Marketo Engage puede enviar una alerta por correo electrónico con información de la persona a cualquier persona: el propietario de ventas, un socio o cualquier otra persona. Utilice el paso de flujo &quot;[!UICONTROL Enviar alerta]&quot;.

![](assets/send-alert-1.png)

1. Busque y seleccione el correo electrónico que desea enviar.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >La alerta de correo electrónico debe contener toda la información del encabezado y estar en el estado **[!UICONTROL Aprobado]**.

1. Puede hacer clic en el icono de previsualización para asegurarse de que ha seleccionado el correo electrónico correcto.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Asegúrese de usar el token &quot;[!UICONTROL Enviar información de alerta]&quot; en el correo electrónico.

1. Seleccione el destinatario de la alerta. Puede elegir [!UICONTROL Propietario de ventas] o [!UICONTROL Propietario de cuenta].

   ![](assets/send-alert-4.png)

1. Opcionalmente, agregue cualquier otra dirección de correo electrónico que desee (separada por una coma o un punto y coma).

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >En campañas de déclencheur, puede usar tokens en **[!UICONTROL Para otros correos electrónicos]** como `{{lead.Territory Owner}}` o `{{my.Alert Recipient}}` siempre que los valores sean direcciones de correo electrónico válidas. Los tokens de **[!UICONTROL Para otros correos electrónicos]** no funcionarán en una campaña por lotes.

>[!MORELIKETHIS]
>
>[Crear un correo electrónico](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
