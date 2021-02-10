---
unique-page-id: 2952678
description: Usar el testigo de información de alerta de envío {{SP_Send_Alert_Info}} - Documentos de marketing - Documentación del producto
title: Usar el testigo Enviar información de alerta
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---


# Usar el testigo Enviar información de alerta {#use-the-send-alert-info-token-sp-send-alert-info}

El token `{{SP_Send_Alert_Info}}` es un token especial que se utiliza al crear correos electrónicos de alerta para su equipo de ventas.

>[!TIP]
>
>Este token sólo funciona como se espera al enviar el correo electrónico que lo contiene con el paso de flujo [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md). No funcionará cuando se utilice en un paso de flujo de correo electrónico de envío.

Ejemplo de alerta:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>¡Cabeza! Las direcciones URL de las alertas tienen fechas de caducidad, por lo que asegúrese de que tienen una cadencia que admita estos tipos de mensajes. Las fechas de caducidad son [configuradas por un administrador](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

La siguiente información se incluye como parte del `{{SP_Send_Alert_Info}}`:

* Nombre y apellidos como vínculo al detalle de la persona en Marketing
* Un vínculo a la persona de su CRM
* El nombre de la campaña en Marketing que envió la alerta
* La hora a la que se envió la alerta

>[!NOTE]
>
>El vínculo a CRM solo aparecerá si la persona está en el sistema CRM (actualmente no disponible con Dynamics CRM). El vínculo es accesible tanto para usuarios de Marketing como para usuarios que no son de Marketing.

## Añadir el token SP_Send_Alert_Info en un mensaje de correo electrónico {#add-the-sp-send-alert-info-token-to-an-email}

1. Seleccione el correo electrónico y haga clic en **Editar borrador**.

   ![](assets/one-3.png)

1. Haga clic con el botón doble en el área editable a la que desee agregar el token.

   ![](assets/two-3.png)

1. Sitúe el cursor donde desee que esté el token y, a continuación, haga clic en el botón **Insertar token**.

   ![](assets/three-3.png)

1. Busque y seleccione el token **`{{SP_Send_Alert_Info}}`** y haga clic en **Insertar**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>No te olvides de aprobar tu correo electrónico.

¡Buenas cosas! Este token es muy útil y debe utilizarlo en todas las alertas que cree para su equipo de ventas.
