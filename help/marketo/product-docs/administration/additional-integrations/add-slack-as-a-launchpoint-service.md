---
unique-page-id: 12983619
description: 'Añadir Slack como servicio de LaunchPoint: Documentos de Marketo: Documentación del producto'
title: Añadir Slack como servicio de LaunchPoint
exl-id: 38c1501d-27ac-4c6c-967d-4decd10e0cb3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Agregar Slack como servicio de LaunchPoint {#add-slack-as-a-launchpoint-service}

La integración del Slack incluye dos tipos de notificación:

* **Notificaciones** del sistema: Obtenga notificaciones del Slack sobre eventos importantes en su instancia de Marketo, como alertas sobre estados de campañas actuales y cualquier problema que requiera atención inmediata (errores de CRM y límites de API).
* **Momentos** interesantes: Cuando una persona conocida ha activado Marketo Insight desde una cuenta de ventas, los propietarios potenciales pueden recibir notificaciones por medio de un Slack. Las notificaciones incluyen información sobre posibles clientes, así como detalles sobre la cuenta de ventas.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!PREREQUISITES]
>
>Si no tiene activadas las Notificaciones del sistema de Slack, póngase en contacto con el [Soporte de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Vaya a **LaunchPoint** y, a continuación, en **Nuevo** haga clic en **Nuevo servicio**.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Introduzca un nombre para mostrar para la integración del Slack. En la lista desplegable **Service**, seleccione **Slack**. Haga clic en **Crear**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Haga clic en **Autorizar**. Esto abre el Slack en una nueva pestaña, donde se completa la autorización y se concede permiso a Marketo para extraer información del Slack.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. En la nueva pestaña del Slack, introduzca la dirección URL del espacio de trabajo y haga clic en **Continue**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Introduzca sus credenciales de Slack y haga clic en **Iniciar sesión**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. En la lista desplegable **Publicar en**, seleccione el canal en el que desea que se publiquen las notificaciones de Marketo. Revise los permisos solicitados y haga clic en **Autorizar**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. Debería ver la pantalla de confirmación a continuación. La pestaña se cierra automáticamente.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Actualice la pestaña Marketo y confirme que el Slack aparece ahora como un servicio activo en LaunchPoint.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   Ahora, las notificaciones empezarán a publicarse en el canal seleccionado en el paso 6. Se parecerán a esto:

   ![](assets/samplenotification.png)
