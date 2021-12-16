---
unique-page-id: 18317340
description: Comprobación de cancelación de suscripción de Marketo - Documentos de Marketo - Documentación del producto
title: Comprobación de cancelación de suscripción de Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
source-git-commit: 82c75d52caf3a0320cd3e8534b3b0870cf12d660
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Comprobación de cancelación de suscripción de Marketo {#marketo-unsubscribe-check}

La comprobación de cancelación de suscripción de Marketo utiliza la conexión de su equipo a Marketo para evitar que los correos electrónicos se dirijan a personas que han dejado de suscribirse en el sistema de administración de posibles clientes de Marketo. Cuando un usuario de ventas envía un correo electrónico con Sales Connect, se realiza una llamada API a Marketo para comprobar si se da de baja el ID de correo electrónico. Si es así, bloquearemos el envío del correo electrónico.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Activándolo {#turning-it-on}

1. En la aplicación web, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/one-2.png)

1. En Configuración de administración, haga clic en **Cancelación de suscripción**.

   ![](assets/two-3.png)

1. Haga clic en **Integraciones**.

   ![](assets/three-3.png)

1. En la sección Marketo Unsubscribe Check , haga clic en el control deslizante para activar la comprobación.

   ![](assets/four-2.png)

## Aspectos importantes {#things-to-know}

La comprobación de cancelación de suscripción de Marketo...

* No cuenta con los límites de su API
* Requiere que se establezca una conexión de Marketo
* Es una configuración global
* Bloquea los correos electrónicos enviados desde la aplicación web, los clientes de correo electrónico y Salesforce
* Registrará un correo electrónico con errores o impedirá que un usuario envíe cuando intente enviar para todos los flujos de trabajo (envío de complemento de correo electrónico, envío individual, envío de campaña de ventas, selección múltiple y envío) excepto para [agrupar correos electrónicos](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), en la que evitaremos que los correos electrónicos se envíen en silencio
