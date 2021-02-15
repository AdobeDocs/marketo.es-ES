---
unique-page-id: 11376159
description: Antes de crear notificaciones push y mensajes en la aplicación - Documentos de marketing - Documentación del producto
title: Antes de crear notificaciones push y mensajes en la aplicación
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# Antes de crear notificaciones push y mensajes en la aplicación {#before-you-create-push-notifications-and-in-app-messages}

La creación de notificaciones push y mensajes en la aplicación no es difícil, pero debe tener todo listo antes de poder realizar el inicio. El administrador de marketing y el desarrollador de aplicaciones móviles deben seguir los pasos a continuación para preparar las integraciones necesarias.

1. En primer lugar, el administrador de marketing [agrega una aplicación móvil](add-a-mobile-app.md)
1. A continuación, el administrador de marketing [envía un fragmento de código al desarrollador](send-sdk-code-to-a-developer.md)
1. El desarrollador descarga el SDK e incluye fragmentos de código y otros métodos para [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) o [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. De forma predeterminada, los mensajes en la aplicación se activan cuando se abre la aplicación. Si desea déclencheur de mensajes para otros eventos, como cuando se ve una página en particular o se pulsa un botón específico, el programador debe agregar eventos personalizados al código (consulte [Eventos personalizados para mensajes en la aplicación](#CustomEvents) más adelante)
1. El desarrollador [genera la clave de API de servidor y el número de proyecto para Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) o [la certificación y contraseña para iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) y la envía al administrador de Marketing to
1. El administrador de marketing configura el acceso de notificaciones push [con la clave de API de servidor (Android)](configure-mobile-app-android-push-access.md) o [con el certificado (iOS)](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>Es fácil para un administrador de marketing comprobar si la configuración push está verificada. Sólo vaya [aquí](verify-push-configuration.md).

## Eventos personalizados para mensajes en la aplicación {#custom-events-for-in-app-messages}

Para la mensajería en la aplicación, el déclencheur de visualización se establece en **Apertura de la aplicación** de forma predeterminada. Si desea utilizar eventos personalizados para déclencheur de la visualización de mensajes en la aplicación (por ejemplo, **Clics que Añaden al carro**, **Página de configuración de Vistas**), cree una lista de los eventos deseados y déselo a su desarrollador de aplicaciones móviles. A continuación, el desarrollador agregará los eventos personalizados al código. Una vez aprobados, aparecen como déclencheur de visualización al configurar la audiencia. **Precaución**: Es posible que el proceso de aprobación de la codificación de evento personalizado tarde algún tiempo en completarse.

Una vez que haya terminado toda la preparación de los mensajes en la aplicación y las notificaciones push, es hora de empezar.

>[!MORELIKETHIS]
>
>* [Crear un mensaje en la aplicación](https://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [Crear una notificación push](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



