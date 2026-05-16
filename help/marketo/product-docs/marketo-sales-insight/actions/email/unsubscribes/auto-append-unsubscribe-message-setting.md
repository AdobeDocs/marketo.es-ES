---
description: Obtenga información sobre cómo habilitar o deshabilitar el mensaje de cancelación de suscripción de anexado automático para correos electrónicos de ventas.
title: Anexar automáticamente la configuración del mensaje de cancelación de suscripción
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
TQID: https://experienceleague.adobe.com/4iAq0-giVwuDcqaoi8QnLN35QO67RSlgHYXFYaUebZg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 5%

---

# Anexar automáticamente la configuración del mensaje de cancelación de suscripción {#auto-append-unsubscribe-message-setting}

Asegúrese de que cada correo electrónico de acciones de Sales Insight enviado incluya un mensaje de cancelación de suscripción para que los destinatarios tengan una opción sencilla de desactivar la comunicación. Cuando se activa el mensaje de cancelación de suscripción de datos anexados, todas las comunicaciones que su equipo envía desde Marketo Sales incluyen un mensaje de cancelación de suscripción, incluidos los correos electrónicos enviados desde la aplicación web y Salesforce.

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
