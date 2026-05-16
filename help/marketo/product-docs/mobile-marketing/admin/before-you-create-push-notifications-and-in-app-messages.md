---
unique-page-id: 11376159
description: Saber qué se debe configurar antes de crear mensajes push y en la aplicación. Obtenga instrucciones para administradores y desarrolladores, SDK y para eventos personalizados.
title: Antes de crear notificaciones push y mensajes en la aplicación
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
TQID: https://experienceleague.adobe.com/YNAyIX3spLETvHChasi9xpP9K96ksYdkr-MSdGp2qog
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 417
ht-degree: 4%

---

# Antes de crear notificaciones push y mensajes en la aplicación {#before-you-create-push-notifications-and-in-app-messages}

Crear notificaciones push y mensajes en la aplicación no es difícil, pero debe tener todo listo antes de empezar. El administrador de Marketo y el desarrollador de aplicaciones móviles deben seguir los pasos a continuación para preparar las integraciones necesarias.

1. Primero, el administrador de Marketo [agrega una aplicación móvil](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. A continuación, el administrador de Marketo [envía un fragmento de código al desarrollador](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. El desarrollador descarga SDK e incluye fragmentos y otros métodos para [Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) o [iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios).

1. De forma predeterminada, los mensajes en la aplicación se activan al abrirse la aplicación. Si desea almacenar en déclencheur mensajes para otros eventos, como cuando se ve una página en particular o se presiona un botón específico, el desarrollador debe agregar eventos personalizados al código (consulte [Eventos personalizados para mensajes en la aplicación](#CustomEvents) más abajo).

1. El desarrollador [genera la clave de API de servidor y el número de proyecto para Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) o [la certificación y la contraseña para iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios) y la envía al administrador de Marketo.

1. El administrador de Marketo configura el acceso a las notificaciones push [con la clave de API del servidor (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) o [con el certificado (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Es fácil para un administrador de Marketo comprobar si la configuración push está verificada. Solo tienes que ir [aquí](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventos personalizados para mensajes en la aplicación {#custom-events-for-in-app-messages}

Para la mensajería en la aplicación, el déclencheur de visualización está establecido en **[!UICONTROL Apertura de aplicación]** de manera predeterminada. Si desea usar eventos personalizados para almacenar en déclencheur la visualización de los mensajes en la aplicación (por ejemplo, **Clics en Agregar al carro de compras**, **Página de configuración de vistas**), cree una lista de los eventos deseados y entréguela al desarrollador de aplicaciones móviles. A continuación, el desarrollador agregará los eventos personalizados al código. Una vez aprobadas, aparecen como déclencheur de visualización al configurar la audiencia. **Precaución**: el proceso de aprobación de la codificación de eventos personalizados puede tardar un poco en completarse.

Después de haber completado toda la preparación para los mensajes en la aplicación y las notificaciones push, es hora de empezar.

>[!MORELIKETHIS]
>
>* [Crear un mensaje en la aplicación](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Crear una notificación push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
