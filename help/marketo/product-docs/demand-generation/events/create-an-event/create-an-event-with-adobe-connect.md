---
unique-page-id: 2949865
description: 'Creación de un evento con Adobe Connect: documentos de Marketo, documentación del producto'
title: Creación de un evento con Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Creación de un evento con Adobe Connect {#create-an-event-with-adobe-connect}

La sincronización con Adobe Connect le permite administrar el registro y la asistencia a seminarios web dentro de Marketo, lo que garantiza que la participación no se quede sin rastrear.

>[!PREREQUISITES]
>
>* [Vincular Adobe Connect y Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

En primer lugar, asegúrese de haber creado la reunión o el seminario en Adobe Connect. Si necesita ayuda, consulte la [Guía del usuario de Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Las reuniones y seminarios que cree en Adobe Connect deben crearse en la carpeta especificada al introducir sus credenciales en Marketo. Después de crear la reunión o el seminario, anote la información logística pertinente (como el número de teléfono) que desee utilizar en el correo electrónico de confirmación y en el archivo ICS.

>[!CAUTION]
>
>Como anfitrión del evento, asegúrese de unirse desde la aplicación y **no** mediante el vínculo enviado a los asistentes.

>[!NOTE]
>
>En este momento no se admite Adobe Connect en el sitio.

1. En la página principal de un nuevo evento, selecciona **[!UICONTROL Acciones de evento]** y, a continuación, **[!UICONTROL Configuración de evento]**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Si no ves **[!UICONTROL Configuración de eventos]** en la lista desplegable, asegúrate de que el canal del evento tenga **[!UICONTROL Evento con seminario web]** seleccionado en &quot;[!UICONTROL Se aplica a]&quot;.

1. En **[!UICONTROL Socio de evento]**, seleccione **[!UICONTROL Adobe Connect]**.

   ![](assets/event-settings-adobe-connect.png)

1. Seleccione su ID de **[!UICONTROL inicio de sesión]** y luego seleccione su **[!UICONTROL evento]**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/event-settings-overview.png)

   ¡Bonito! El evento de Adobe Connect ahora se sincroniza con el evento de Marketo.

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellidos, Dirección de correo electrónico.

   >[!TIP]
   >
   >Para insertar la dirección URL única de la persona en un correo electrónico, use este token: `{{member.webinar url}}`. Cuando se envía el correo electrónico, este token resuelve automáticamente la URL de confirmación única de la persona desde Adobe Connect.
   >
   >Establece tu correo electrónico de confirmación en **Operativo** para asegurarte de que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

   Las personas que se suscriban a tu seminario web se transferirán a tu proveedor de seminarios web a través del paso de flujo [!UICONTROL Cambiar estado del programa] cuando el [!UICONTROL Nuevo estado] se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de hacer que el paso de flujo [!UICONTROL Cambiar estado del programa] #1 y el paso de flujo [!UICONTROL Enviar correo electrónico] #2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de tanto tiempo aún no ves nada, selecciona **[!UICONTROL Actualizar del proveedor de seminarios web]** en el menú Acciones de eventos de la pestaña Resumen del evento.

   >[!MORELIKETHIS]
   >
   >* [Agregar Adobe Connect as a [!DNL LaunchPoint] Service](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Editar un canal de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
