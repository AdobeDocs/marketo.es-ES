---
unique-page-id: 11376159
description: Antes de crear notificaciones push y mensajes en la aplicación - Documentos de Marketo - Documentación del producto
title: Antes de crear notificaciones push y mensajes en la aplicación
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Antes de crear notificaciones push y mensajes en la aplicación {#before-you-create-push-notifications-and-in-app-messages}

La creación de notificaciones push y mensajes en la aplicación no es difícil, pero debe tener todo listo antes de empezar. El administrador de Marketo y el desarrollador de aplicaciones móviles deben seguir los pasos a continuación para preparar las integraciones necesarias.

1. En primer lugar, el administrador de Marketo [agrega una aplicación móvil](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. A continuación, el administrador de Marketo [envía un fragmento de código al desarrollador](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. El desarrollador descarga el SDK e incluye fragmentos de código y otros métodos para [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) o [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. De forma predeterminada, los mensajes en la aplicación se activan al abrirse la aplicación. Si desea almacenar en déclencheur mensajes para otros eventos, como cuando se ve una página en particular o se presiona un botón específico, el desarrollador debe agregar eventos personalizados al código (consulte [Eventos personalizados para mensajes en la aplicación](#CustomEvents) más abajo).

1. El desarrollador [genera la clave de API del servidor y el número de proyecto para Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) o [certificación y contraseña para iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) y lo envía al administrador de Marketo.

1. El administrador de Marketo configura el acceso de notificaciones push [con la clave de API del servidor (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) o [con el certificado (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Un administrador de Marketo puede comprobar fácilmente si la configuración push está verificada. Solo vete [here](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventos personalizados para mensajes en la aplicación {#custom-events-for-in-app-messages}

Para la mensajería en la aplicación, el déclencheur de visualización se establece en **Apertura de la aplicación** de forma predeterminada. Si desea utilizar cualquier evento personalizado para almacenar en déclencheur la visualización de mensajes en la aplicación (por ejemplo, **Clics Agregar al carro**, **Página Configuración de vistas**), cree una lista de los eventos que desee y asígnelo a su desarrollador de aplicaciones móviles. El desarrollador agrega los eventos personalizados al código. Una vez aprobadas, aparecen como déclencheur de visualización al configurar la audiencia. **Precaución**: El proceso de aprobación de la codificación de eventos personalizada puede tardar algún tiempo en completarse.

Una vez que haya hecho toda la preparación para los mensajes en la aplicación y las notificaciones push, es hora de empezar.

>[!MORELIKETHIS]
>
>* [Crear un mensaje en la aplicación](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Creación de una notificación push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

