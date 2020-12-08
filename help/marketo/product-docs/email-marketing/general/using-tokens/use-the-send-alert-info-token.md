---
unique-page-id: 2952678
description: Usar el testigo de información de alerta de envío {{SP_Send_Alert_Info}} - Documentos de marketing - Documentación del producto
title: Usar el testigo Enviar información de alerta
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---


# Usar el testigo Enviar información de alerta {#use-the-send-alert-info-token-sp-send-alert-info}

El `{{SP_Send_Alert_Info}}` token es un token especial que se utiliza al crear mensajes de correo electrónico de alerta para el equipo de ventas.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!TIP]
>
>Este token solo funciona como se espera al enviar el correo electrónico que lo contiene con el paso [Enviar alerta](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) . No funcionará cuando se utilice en un paso de flujo de correo electrónico de envío.

Ejemplo de alerta:   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>¡Cabeza! Las direcciones URL de las alertas tienen fechas de caducidad, por lo que asegúrese de que tienen una cadencia que admita estos tipos de mensajes. Las fechas de caducidad las [configura un administrador](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

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

1. Sitúe el cursor donde desee que esté el token y, a continuación, haga clic en el botón **Insertar token** .

   ![](assets/three-3.png)

1. Busque y seleccione el **`{{SP_Send_Alert_Info}}`** token y haga clic en **Insertar**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**Recordatorio**
>
>No te olvides de aprobar tu correo electrónico.

¡Buenas cosas! Este token es muy útil y debe utilizarlo en todas las alertas que cree para su equipo de ventas.