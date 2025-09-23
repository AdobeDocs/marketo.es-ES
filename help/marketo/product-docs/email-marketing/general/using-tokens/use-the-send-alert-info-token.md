---
unique-page-id: 2952678
description: Usar el token para enviar información de alerta {{SP_Send_Alert_Info}} - Documentos de Marketo - Documentación del producto
title: Usar el token de información de envío de alerta
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 5%

---

# Usar el token de información de envío de alerta {#use-the-send-alert-info-token-sp-send-alert-info}

El token `{{SP_Send_Alert_Info}}` es un token especial que se utilizará al crear correos electrónicos de alerta para su equipo de ventas.

>[!TIP]
>
>Este token solo funciona según lo previsto al enviar el correo electrónico que lo contiene con el paso de flujo [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md). No funcionará cuando se utilice en un paso Enviar flujo de correo electrónico.

Ejemplo de alerta:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>¡Cuidado! Las direcciones URL de las alertas tienen fechas de caducidad, por lo que debe asegurarse de que tengan una cadencia que admita este tipo de mensajes. Las fechas de caducidad son [configuradas por un administrador](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

La siguiente información se incluye como parte de `{{SP_Send_Alert_Info}}`:

* Nombre y apellidos como vínculo al detalle de persona en Marketo
* Un vínculo a la persona en su CRM
* Nombre de la campaña en Marketo que envió la alerta
* La hora a la que se envió la alerta

>[!NOTE]
>
>El vínculo a CRM solo aparecerá si la persona está en el sistema CRM (actualmente no disponible con Dynamics CRM). El vínculo es accesible tanto para los usuarios de Marketo como para los que no son de Marketo.

## Agregar el token SP_Send_Alert_Info a un correo electrónico {#add-the-sp-send-alert-info-token-to-an-email}

1. Seleccione el correo electrónico y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/one-3.png)

1. Haga doble clic en el área editable donde desee agregar el token.

   ![](assets/two-3.png)

1. Coloque el cursor donde desee que esté el token y, a continuación, haga clic en el botón **[!UICONTROL Insertar token]**.

   ![](assets/three-3.png)

1. Busque y seleccione el token **[!UICONTROL {{SP_Send_Alert_Info}}]**, y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>No olvide aprobar su correo electrónico.

¡Muy bien! Este token es muy útil y debe utilizarlo en todas las alertas que cree para su equipo de ventas.
