---
description: Configuración del mensaje de cancelación de suscripción anexada automáticamente - Documentos de Marketo - Documentación del producto
title: Anexar automáticamente la configuración del mensaje de cancelación de suscripción
hide: true
hidefromtoc: true
feature: Sales Insight Actions
source-git-commit: 8b2eed5e28c46ea9c467fd25dd732c1654a09bed
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Anexar automáticamente la configuración del mensaje de cancelación de suscripción {#auto-append-unsubscribe-message-setting}

Asegúrese de que cada correo electrónico de acciones de información de ventas enviado incluya un mensaje de cancelación de suscripción para que los destinatarios tengan una opción fácil de desactivar la comunicación. Cuando se habilita el mensaje de cancelación de suscripción de datos anexados, todas las comunicaciones que su equipo envía desde Marketo Sales incluyen un mensaje de cancelación de suscripción, incluidos los correos electrónicos enviados desde la aplicación web y Salesforce.

>[!NOTE]
>
>Si usa el `{{team_unsubscribe}}` campo dinámico en una plantilla de correo electrónico y la configuración cancelar la suscripción del mensaje anexado está habilitada, el campo dinámico cancelar la suscripción del equipo rellenará el mensaje cancelar la suscripción _en lugar de_ adjuntando el mensaje de cancelación de suscripción.

## Habilitar/deshabilitar la adición de cancelación de suscripción {#enable-disable-unsubscribe-append}

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. En Configuración De Administración, Haga Clic En **Cancela la suscripción**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. En la pestaña Mensajería, en Anexar mensaje de cancelación de suscripción, mueva el control deslizante al estado deseado.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Si desactiva la configuración del mensaje de cancelación de suscripción de datos anexados, le recomendamos que agregue un pie de página de cancelación de suscripción a las plantillas para garantizar que la comunicación tenga una opción de exclusión. Para ello, agregue su propio mensaje personalizado a cada plantilla o utilice el `{{team_unsubscribe}}` [campo dinámico](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
