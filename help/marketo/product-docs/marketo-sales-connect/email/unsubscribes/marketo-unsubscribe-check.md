---
unique-page-id: 18317340
description: Comprobación de cancelación de suscripción de Marketo - Documentos de Marketo - Documentación del producto
title: Verificación de cancelación de suscripción de Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---

# Verificación de cancelación de suscripción de Marketo {#marketo-unsubscribe-check}

La comprobación de cancelación de suscripción de Marketo utiliza la conexión de su equipo a Marketo para evitar que los correos electrónicos lleguen a personas que han cancelado su suscripción en el sistema de administración de posibles clientes de Marketo. Cuando un usuario de ventas envía un correo electrónico con Sales Connect, se realiza una llamada de API a Marketo para comprobar si se ha cancelado la suscripción del ID de correo electrónico. Si es así, bloquearemos el envío del correo electrónico.

>[!NOTE]
>
>**Permisos de administración necesarios**

## Encendiéndola... {#turning-it-on}

1. En la aplicación web, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/one-2.png)

1. En Configuración de administración, haga clic en **Cancela la suscripción**.

   ![](assets/two-3.png)

1. Clic **Integraciones**.

   ![](assets/three-3.png)

1. En la sección Cancelar la suscripción a Marketo, haga clic en el control deslizante para activar la comprobación.

   ![](assets/four-2.png)

## Cosas que saber {#things-to-know}

Comprobación de cancelación de suscripción de Marketo...

* No cuenta con sus límites de API
* Requiere que se establezca una conexión de Marketo
* Es una configuración global
* Bloquea los correos electrónicos enviados desde la aplicación web, los clientes de correo electrónico y Salesforce
* Registrará un correo electrónico con errores o evitará que un usuario envíe mensajes cuando intente enviarlos para todos los flujos de trabajo (envío de complemento de correo electrónico, envío individual, envío de campaña de ventas, selección múltiple y envío) excepto para [agrupar correos electrónicos](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), en el que evitaremos que los correos electrónicos se envíen en silencio
