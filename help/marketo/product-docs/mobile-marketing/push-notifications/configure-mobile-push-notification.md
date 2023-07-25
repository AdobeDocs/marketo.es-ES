---
unique-page-id: 7512454
description: 'Configuración de notificaciones push móviles: documentos de Marketo, documentación del producto'
title: Configuración de notificaciones push móviles
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Configuración de notificaciones push móviles {#configure-mobile-push-notification}

1. Vaya a la **Actividades de marketing** área.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Seleccione el recurso push y haga clic en **Editar borrador**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Ir a **Configurar**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Seleccione la aplicación que desee. Las plataformas Android y Apple están habilitadas de forma predeterminada.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Si el mensaje push se aplica solo a una plataforma (por ejemplo, en el caso de los iPhone), puede excluir la otra plataforma desplazando su selector a Deshabilitado.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Clic **Siguiente**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Introduzca el texto del mensaje o seleccione el icono de token para añadir tokens. A continuación, seleccione una **Acción de toque**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Si una plataforma está habilitada, aparecerá en la parte izquierda de la pantalla del teléfono. Se muestra en color cuando se selecciona.

   >[!NOTE]
   >
   >Existen tres tipos de acciones de toque:
   >
   >**Iniciar aplicación** - **Esta aplicación** abre la página principal de la aplicación cuando se pulsa la notificación. **Personalizado** utiliza un vínculo profundo para abrir otras áreas de la aplicación o de cualquier otra aplicación a la que tenga el vínculo (consulte [URI de vínculos profundos](#Deeplink) para más detalles).
   >
   >**Página de aterrizaje** : le lleva a una página de aterrizaje de Marketo especificada.
   >
   >**URL externa** : le lleva a una página de aterrizaje que no es de Marketo.

1. Para insertar un vínculo profundo para una acción de toque personalizada, haga clic en Personalizado e introduzca el [URI de vínculo profundo](#Deeplink) en el campo.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Para insertar tokens, seleccione un token, introduzca un valor predeterminado y haga clic en Insertar.

   >[!NOTE]
   >
   >Los tokens aparecen donde se coloca el cursor en el cuadro de texto. Puede utilizar más de un token.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Los mensajes y las acciones táctiles tendrán el mismo aspecto en ambas plataformas.

1. Solo para iOS, marque la casilla de verificación para indicar a la aplicación que reproduzca un sonido cuando reciba el mensaje. Android reproduce el sonido automáticamente.

   ![](assets/ios-tap-and-notification-hand.png)

1. Previsualice la otra plataforma y haga clic en **Finalizar**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Clic **Aprobar y cerrar**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

¡Felicidades! Ahora la notificación push está lista para enviarse.

## URI de vínculos profundos {#deep-link-uris}

Cuando los suscriptores hacen clic en un botón de un mensaje push, puede llevarlos a la página de inicio de la aplicación o directamente a una página específica dentro de la aplicación. Un vínculo profundo es una referencia única a una página específica de la aplicación y se parece mucho a un vínculo a un sitio web.

Un URI de vínculo profundo consta de tres partes: nombre del esquema, ruta e identificador. En el ejemplo siguiente, &quot;myappname&quot; es el esquema. &quot;products&quot; es la ruta y &quot;purple-shirt&quot; es el identificador. Cuando el cliente pulse, se le redirigirá específicamente al elemento de camisa morada dentro de las páginas de producto de la aplicación.

![](assets/image2016-7-29-12-3a49-3a1.png)

Dicho esto, la estructura de vínculos profundos de su aplicación puede ser diferente del ejemplo anterior. El desarrollador tiene muchas opciones para definir URI de vínculos profundos, por lo que debe pedirle que le envíe los URI (vínculos) de las páginas que le interesen. Esto garantizará que las URI que introduzca en los mensajes push apunten a los lugares correctos. El desarrollador puede [encuentre más información aquí](https://developers.marketo.com/mobile/enabling-deep-links-in-your-app/).

>[!MORELIKETHIS]
>
>[Enviar una notificación push móvil](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
