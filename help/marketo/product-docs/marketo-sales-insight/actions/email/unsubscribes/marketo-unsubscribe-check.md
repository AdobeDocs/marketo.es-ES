---
description: Comprobación de cancelación de suscripción de Marketo - Documentos de Marketo - Documentación del producto
title: Verificación de cancelación de suscripción de Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---

# [!UICONTROL Comprobación de cancelación de suscripción de Marketo] {#marketo-unsubscribe-check}

La [!UICONTROL comprobación de cancelación de suscripción de Marketo] usa la conexión de su equipo con Marketo para evitar que los mensajes de correo electrónico se envíen a personas que cancelaron su suscripción en el sistema de administración de posibles clientes de Marketo. Cuando un usuario de ventas envía un correo electrónico con [!DNL Marketo Sales], se realiza una llamada de API a Marketo para comprobar si se cancela la suscripción del ID de correo electrónico. Si es así, bloquearemos el envío del correo electrónico.

>[!NOTE]
>
>**Se requieren permisos de administración**

## Encendiéndola... {#turning-it-on}

1. Haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL Cancelar suscripciones]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Haga clic en la ficha **[!UICONTROL Integraciones]**. En la sección [!UICONTROL Comprobación de cancelación de suscripción de Marketo], haga clic en el control deslizante para activar la comprobación.

   ![](assets/marketo-unsubscribe-check-3.png)

## Cosas que saber {#things-to-know}

Comprobación de cancelación de suscripción de Marketo...

* No cuenta con sus límites de API
* Requiere que se establezca una conexión de Marketo
* Es una configuración global
* Bloquea los correos electrónicos enviados desde la aplicación web, los clientes de correo electrónico y [!DNL Salesforce]
