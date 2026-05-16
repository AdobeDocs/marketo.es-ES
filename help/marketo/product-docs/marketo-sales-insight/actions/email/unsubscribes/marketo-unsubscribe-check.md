---
description: Consulta la casilla de cancelación de suscripción de Marketo para que los vendedores no puedan enviar correos electrónicos a las personas que cancelaron la suscripción en Marketo.
title: Verificar cancelación de suscripción de Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/RaIYKEVyjdeUlOa4paltYIS8NPZHi1XWTmO4IeLBy-o
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 6%

---

# [!UICONTROL Comprobación de cancelación de suscripción de Marketo] {#marketo-unsubscribe-check}

La [!UICONTROL comprobación de cancelación de suscripción de Marketo] usa la conexión de su equipo con Marketo para evitar que los mensajes de correo electrónico se envíen a personas que cancelaron su suscripción en el sistema de administración de posibles clientes de Marketo. Cuando un usuario de ventas envía un correo electrónico con [!DNL Marketo Sales], se realiza una llamada de API a Marketo para comprobar si se cancela la suscripción del ID de correo electrónico. Si es así, bloquearemos el envío del correo electrónico.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Encendiéndola... {#turning-it-on}

1. Haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL Cancelar suscripciones]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Haga clic en la ficha **[!UICONTROL Integraciones]**. En la sección [!UICONTROL Comprobación de cancelación de suscripción de Marketo], haga clic en el control deslizante para activar la comprobación.

   ![](assets/marketo-unsubscribe-check-3.png)

## Cosas que debe saber {#things-to-know}

Comprobación de cancelación de suscripción de Marketo...

* No cuenta con sus límites de API
* Requiere que se establezca una conexión de Marketo
* Es una configuración global
* Bloquea los correos electrónicos enviados desde la aplicación web, los clientes de correo electrónico y [!DNL Salesforce]
