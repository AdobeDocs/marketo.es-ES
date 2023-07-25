---
unique-page-id: 11376159
description: 'Antes de crear notificaciones push y mensajes en la aplicación: documentos de Marketo, documentación del producto'
title: Antes de crear notificaciones push y mensajes en la aplicación
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Antes de crear notificaciones push y mensajes en la aplicación {#before-you-create-push-notifications-and-in-app-messages}

La creación de notificaciones push y mensajes en la aplicación no es difícil, pero debe tener todo listo antes de empezar. El administrador de Marketo y el desarrollador de aplicaciones móviles deben seguir los pasos a continuación para preparar las integraciones necesarias.

1. Primero, el administrador de Marketo [añade una aplicación móvil](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. A continuación, el administrador de Marketo [envía un fragmento de código al desarrollador](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. El desarrollador descarga el SDK e incluye fragmentos de código y otros métodos para [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) o [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. De forma predeterminada, los mensajes en la aplicación se activan al abrirse la aplicación. Si desea almacenar en déclencheur mensajes para otros eventos, como cuando se visualiza una página en particular o se pulsa un botón específico, el desarrollador debe añadir eventos personalizados al código (consulte [Eventos personalizados para mensajes en la aplicación](#CustomEvents) abajo).

1. El desarrollador [genera la clave de API de servidor y el número de proyecto para Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) o [la certificación y la contraseña de iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) y lo envía al administrador de Marketo.

1. El administrador de Marketo configura el acceso a las notificaciones push [con la clave de API del servidor (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) o [con el certificado (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Es fácil para un administrador de Marketo comprobar si la configuración push está verificada. Solo vete [aquí](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventos personalizados para mensajes en la aplicación {#custom-events-for-in-app-messages}

Para la mensajería en la aplicación, el déclencheur de visualización se establece en **Apertura de aplicación** de forma predeterminada. Si desea utilizar eventos personalizados para almacenar en déclencheur la visualización de los mensajes en la aplicación (por ejemplo, **Clics Añadir al carro**, **Página Configuración de vistas**), cree una lista de los eventos deseados y entréguela al desarrollador de aplicaciones móviles. A continuación, el desarrollador agregará los eventos personalizados al código. Una vez aprobadas, aparecen como déclencheur de visualización al configurar la audiencia. **Precaución**: el proceso de aprobación de la codificación de evento personalizado puede tardar algún tiempo en completarse.

Después de haber completado toda la preparación para los mensajes en la aplicación y las notificaciones push, es hora de empezar.

>[!MORELIKETHIS]
>
>* [Creación de un mensaje en la aplicación](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Crear una notificación push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
