---
unique-page-id: 18317340
description: Comprobación de cancelación de la suscripción a Marketing - Documentos de marketing - Documentación del producto
title: Comprobación de cancelación de suscripción a Marketing
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Comprobación de cancelación de suscripción de marketing {#marketo-unsubscribe-check}

La comprobación de cancelación de suscripciones de Marketing utiliza la conexión de su equipo con Marketing para evitar que los correos electrónicos se dirijan a personas que no están suscritas en el sistema de gestión de posibles clientes de Marketing. Cuando un usuario de ventas envía un correo electrónico con Sales Connect, se realiza una llamada de API a Marketing para comprobar si se ha cancelado la suscripción al ID de correo electrónico. Si es así, bloquearemos el envío del correo electrónico.

>[!NOTE]
>
>**Se requieren permisos de administración**

## Activándolo {#turning-it-on}

1. En la aplicación web, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/one-2.png)

1. En Configuración de administración, haga clic en **Cancelar suscripciones**.

   ![](assets/two-3.png)

1. Haga clic en **Integraciones**.

   ![](assets/three-3.png)

1. En la sección Marketo Cancelar suscripción, haga clic en el deslizador para activar la marca.

   ![](assets/four-2.png)

## Cosas que hay que saber {#things-to-know}

La comprobación de cancelación de suscripción de Marketing to...

* No cuenta con los límites de la API
* Requiere que se establezca una conexión de marketing
* Es un ajuste global
* Bloquea los correos electrónicos enviados desde la aplicación web, los clientes de correo electrónico y Salesforce
