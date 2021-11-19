---
description: Comprobación de cancelación de suscripción de Marketo - Documentos de Marketo - Documentación del producto
title: Comprobación de cancelación de suscripción de Marketo
hide: true
hidefromtoc: true
source-git-commit: a4a92f2d557581d6685342f45c11c260cf9cad3b
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Comprobación de cancelación de suscripción de Marketo {#marketo-unsubscribe-check}

La comprobación de cancelación de suscripción de Marketo utiliza la conexión de su equipo a Marketo para evitar que los correos electrónicos se dirijan a personas que han dejado de suscribirse en el sistema de administración de posibles clientes de Marketo. Cuando un usuario de ventas envía un correo electrónico con ventas de Marketo, se realiza una llamada API a Marketo para comprobar si se da de baja el ID de correo electrónico. Si es así, bloquearemos el envío del correo electrónico.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Activándolo {#turning-it-on}

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. En Configuración de administración, haga clic en **Cancelación de suscripción**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Haga clic en el **Integraciones** pestaña . En la sección Marketo Unsubscribe Check , haga clic en el control deslizante para activar la comprobación.

   ![](assets/marketo-unsubscribe-check-3.png)

## Aspectos importantes {#things-to-know}

La comprobación de cancelación de suscripción de Marketo...

* No cuenta con los límites de su API
* Requiere que se establezca una conexión de Marketo
* Es una configuración global
* Bloquea los correos electrónicos enviados desde la aplicación web, los clientes de correo electrónico y Salesforce
