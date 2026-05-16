---
unique-page-id: 18317340
description: Información sobre la cancelación de la suscripción a Marketo en Sales Connect. Descubra cómo Sales Connect respeta el estado de cancelación de suscripción de Marketo al realizar envíos.
title: Verificar cancelación de suscripción de Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/ZowbVUMoJ8xNXBl47SJDZWpYvjfkAP90xPT1d6dQdPA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 201
ht-degree: 5%

---

# Verificar cancelación de suscripción de Marketo {#marketo-unsubscribe-check}

La [!UICONTROL comprobación de cancelación de suscripción de Marketo] usa la conexión de su equipo con Marketo para evitar que los mensajes de correo electrónico se envíen a personas que cancelaron su suscripción en el sistema de administración de posibles clientes de Marketo. Cuando un usuario de ventas envía un correo electrónico con [!DNL Sales Connect], se realiza una llamada de API a Marketo para comprobar si se cancela la suscripción del ID de correo electrónico. Si es así, bloquearemos el envío del correo electrónico.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Encendiéndola... {#turning-it-on}

1. En la aplicación web, haga clic en el icono de engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/one-2.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL Cancelar suscripciones]**.

   ![](assets/two-3.png)

1. Haga clic en **[!UICONTROL Integraciones]**.

   ![](assets/three-3.png)

1. En la sección [!UICONTROL Comprobación de cancelación de suscripción de Marketo], haga clic en el control deslizante para activar la comprobación.

   ![](assets/four-2.png)

## Cosas que debe saber {#things-to-know}

Comprobación de cancelación de suscripción de Marketo...

* No cuenta con sus límites de API
* Requiere que se establezca una conexión de Marketo
* Es una configuración global
* Bloquea los correos electrónicos enviados desde la aplicación web, los clientes de correo electrónico y Salesforce
* Registrará un correo electrónico con errores o evitará que un usuario envíe mensajes cuando intente enviarlos para todos los flujos de trabajo (envío de complemento de correo electrónico, envío individual, envío de campaña de ventas, selección múltiple y envío) excepto para [correos electrónicos de grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), en los que evitaremos que los correos electrónicos se envíen en silencio
