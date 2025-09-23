---
unique-page-id: 7512454
description: 'Configuración de notificaciones push móviles: documentos de Marketo, documentación del producto'
title: Configurar notificación push para dispositivos móviles
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 3%

---

# Configurar notificación push para dispositivos móviles {#configure-mobile-push-notification}

1. Vaya al área **[!UICONTROL Actividades de marketing]**.

   ![](assets/configure-mobile-push-notification-1.png)

1. Seleccione su recurso push y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/configure-mobile-push-notification-2.png)

1. En **Configuración**, seleccione la aplicación que desee. Las plataformas Android y Apple están habilitadas de forma predeterminada.

   ![](assets/configure-mobile-push-notification-3.png)

   >[!NOTE]
   >
   >Si el mensaje push solo se aplica a una plataforma (por ejemplo, iOS), puede excluir la otra plataforma deslizando manualmente su selector a **Deshabilitado**.

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/configure-mobile-push-notification-4.png)

1. Escriba el texto del mensaje o seleccione el icono de token para agregar tokens (en este editor, a los tokens se les da formato [como suelen tener](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md); puede usar varios tokens). Seleccione una **acción táctil**.

   ![](assets/configure-mobile-push-notification-5.png)

   >[!NOTE]
   >
   >Si una plataforma está habilitada, aparecerá en la parte izquierda de la pantalla del teléfono. Se muestra en color cuando se selecciona.

   >[!NOTE]
   >
   >Existen tres tipos de [!UICONTROL acciones de punteo]:
   >
   >**Iniciar aplicación** - **Esta aplicación** abre la página principal de la aplicación cuando se pulsa la notificación. **Personalizado** usa un vínculo profundo para abrir otras áreas de la aplicación o de cualquier otra aplicación a la que tengas el vínculo (consulta [URI de vínculo profundo](#deep-link-uris) más abajo para obtener detalles).
   >
   >**[!UICONTROL Página de aterrizaje]**: le lleva a una página de aterrizaje de Marketo especificada.
   >
   >**[!UICONTROL Dirección URL externa]**: lo lleva a una página de aterrizaje que no es de Marketo.

1. Para insertar un vínculo profundo para una acción de toque personalizada, selecciona **Personalizado** e introduce el [URI de vínculo profundo](#deep-link-uris) en el campo.

   ![](assets/configure-mobile-push-notification-6.png)

   >[!NOTE]
   >
   >Los mensajes y las acciones táctiles tendrán el mismo aspecto en ambas plataformas.

1. Solo para iOS, marque la casilla de verificación para indicar a la aplicación que reproduzca un sonido cuando reciba el mensaje. Android reproduce el sonido automáticamente.

   ![](assets/configure-mobile-push-notification-7.png)

1. Previsualice la otra plataforma y haga clic en **[!UICONTROL Finalizar]**.

   ![](assets/configure-mobile-push-notification-8.png)

1. Haga clic en **[!UICONTROL Aprobar y cerrar]**.

   ![](assets/configure-mobile-push-notification-9.png)

¡Felicidades! Ahora la notificación push está lista para enviarse.

## URI de vínculos profundos {#deep-link-uris}

Cuando los suscriptores hacen clic en un botón de un mensaje push, puede llevarlos a la página principal de la aplicación o directamente a una página específica de la aplicación. Un vínculo profundo es una referencia única a una página específica de la aplicación y se parece mucho a un vínculo a un sitio web.

Un URI de vínculo profundo consta de tres partes: nombre del esquema, ruta e identificador. En el ejemplo siguiente, &quot;myappname&quot; es el esquema. &quot;products&quot; es la ruta y &quot;purple-shirt&quot; es el identificador. Cuando el cliente pulse, se le redirigirá específicamente al elemento de camisa morada dentro de las páginas de producto de la aplicación.

![](assets/configure-mobile-push-notification-10.png)

Dicho esto, la estructura de vínculos profundos de la aplicación puede ser diferente del ejemplo anterior. El desarrollador tiene muchas opciones para definir URI de vínculos profundos, por lo que debe pedirle que le envíe los URI (vínculos) de las páginas que le interesen. Esto garantizará que las URI que introduzca en los mensajes push apunten a los lugares correctos. Su desarrollador puede [encontrar más información aquí](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Enviar una notificación push móvil](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
