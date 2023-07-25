---
unique-page-id: 2952678
description: Usar el token Enviar información de alerta {{SP_Send_Alert_Info}} - Documentos de Marketo - Documentación del producto
title: Usar el token Enviar información de alerta
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Usar el token Enviar información de alerta {#use-the-send-alert-info-token-sp-send-alert-info}

El `{{SP_Send_Alert_Info}}` token es un token especial que se utiliza para crear correos electrónicos de alerta para su equipo de ventas.

>[!TIP]
>
>Este token solo funciona como se pretende cuando se envía el correo electrónico que lo contiene con el [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) paso de flujo. No funcionará cuando se utilice en un paso Enviar flujo de correo electrónico.

Ejemplo de alerta:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>¡Cuidado! Las direcciones URL de las alertas tienen fechas de caducidad, por lo que debe asegurarse de que tengan una cadencia que admita este tipo de mensajes. Las fechas de caducidad son [configurado por un administrador](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

La siguiente información se incluye como parte de la `{{SP_Send_Alert_Info}}`:

* Nombre y apellidos como vínculo al detalle de persona en Marketo
* Un vínculo a la persona en su CRM
* Nombre de la campaña en Marketo que envió la alerta
* La hora a la que se envió la alerta

>[!NOTE]
>
>El vínculo a CRM solo aparecerá si la persona está en el sistema CRM (actualmente no disponible con Dynamics CRM). El vínculo es accesible tanto para los usuarios de Marketo como para los que no son de Marketo.

## Agregar el token SP_Send_Alert_Info a un correo electrónico {#add-the-sp-send-alert-info-token-to-an-email}

1. Seleccione el correo electrónico y haga clic en **Editar borrador**.

   ![](assets/one-3.png)

1. Haga doble clic en el área editable donde desee agregar el token.

   ![](assets/two-3.png)

1. Coloque el cursor donde desee que esté el token y haga clic en el icono **Insertar token** botón.

   ![](assets/three-3.png)

1. Busque y seleccione el **`{{SP_Send_Alert_Info}}`** token y clic **Insertar**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Clic **Guardar**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>No olvide aprobar su correo electrónico.

¡Muy bien! Este token es muy útil y debe utilizarlo en todas las alertas que cree para su equipo de ventas.
