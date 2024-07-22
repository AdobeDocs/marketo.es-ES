---
description: Configuración del mensaje de cancelación de suscripción anexada automáticamente - Documentos de Marketo - Documentación del producto
title: Anexar automáticamente la configuración del mensaje de cancelación de suscripción
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Anexar automáticamente la configuración del mensaje de cancelación de suscripción {#auto-append-unsubscribe-message-setting}

Asegúrese de que cada correo electrónico de acciones de información de ventas enviado incluya un mensaje de cancelación de suscripción para que los destinatarios tengan una opción fácil de desactivar la comunicación. Cuando se habilita el mensaje de cancelación de suscripción de datos anexados, todas las comunicaciones que su equipo envía desde Marketo Sales incluyen un mensaje de cancelación de suscripción, incluidos los correos electrónicos enviados desde la aplicación web y Salesforce.

>[!NOTE]
>
>Si usa el campo dinámico `{{team_unsubscribe}}` en una plantilla de correo electrónico y la opción de anexar el mensaje de cancelación de suscripción está habilitada, el campo dinámico de cancelación de suscripción del equipo rellenará el mensaje de cancelación de suscripción _en lugar de_ anexando el mensaje de cancelación de suscripción.

## Habilitar/deshabilitar la adición de cancelación de suscripción {#enable-disable-unsubscribe-append}

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. En Configuración De Administración, Haga Clic En **Cancelar Suscripciones**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. En la pestaña Mensajería, en Anexar mensaje de cancelación de suscripción, mueva el control deslizante al estado deseado.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Si desactiva la configuración del mensaje de cancelación de suscripción de datos anexados, le recomendamos que agregue un pie de página de cancelación de suscripción a las plantillas para garantizar que la comunicación tenga una opción de exclusión. Puede hacerlo agregando su propio mensaje personalizado a cada plantilla o utilizando el `{{team_unsubscribe}}` [campo dinámico](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
