---
unique-page-id: 2949865
description: Obtenga información sobre cómo crear un evento con Adobe Connect en Marketo. Configure la integración y sincronice los datos de registro y asistencia.
title: Crear un evento con Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
TQID: https://experienceleague.adobe.com/I6k5QNBRUFdvHu-7xQMolmzHeyVYt-0ajZ0jV-HIPFY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 425
ht-degree: 3%

---

# Crear un evento con Adobe Connect {#create-an-event-with-adobe-connect}

La sincronización con Adobe Connect le permite administrar el registro y la asistencia a seminarios web dentro de Marketo, lo que garantiza que la participación no se quede sin rastrear.

>[!PREREQUISITES]
>
>* [Vincular Adobe Connect y Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

En primer lugar, compruebe que ha creado la reunión o el seminario en Adobe Connect. Si necesita ayuda, consulte la [Guía del usuario de Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Las reuniones y seminarios que cree en Adobe Connect deben crearse en la carpeta especificada al introducir sus credenciales en Marketo. Después de crear la reunión o el seminario, anote la información logística pertinente (como el número de teléfono) que desee utilizar en el correo electrónico de confirmación y en el archivo ICS.

>[!CAUTION]
>
>Como anfitrión del evento, únase desde la aplicación y **no** mediante el vínculo enviado a los asistentes.

>[!NOTE]
>
>Adobe Connect On-Site no es compatible en este momento.

1. En la página principal de un nuevo evento, selecciona **[!UICONTROL Acciones de evento]** y, a continuación, **[!UICONTROL Configuración de evento]**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Si no ve **[!UICONTROL Configuración de eventos]** en la lista desplegable, compruebe que el canal del evento tenga **[!UICONTROL Evento con seminario web]** seleccionado en &quot;[!UICONTROL Se aplica a]&quot;.

1. En **[!UICONTROL Socio de evento]**, seleccione **[!UICONTROL Adobe Connect]**.

   ![](assets/event-settings-adobe-connect.png)

1. Seleccione su ID de **[!UICONTROL inicio de sesión]** y luego seleccione su **[!UICONTROL evento]**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/event-settings-overview.png)

   El evento de Adobe Connect ahora se sincroniza con el evento de Marketo.

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellidos, Dirección de correo electrónico.

   >[!TIP]
   >
   >Para insertar la dirección URL única de la persona en un correo electrónico, use este token: `{{member.webinar url}}`. Cuando se envía el correo electrónico, este token resuelve automáticamente la URL de confirmación única de la persona desde Adobe Connect.
   >
   >Establece tu correo electrónico de confirmación en **Operativo** para asegurarte de que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

   Las personas que se suscriban a tu seminario web se transferirán a tu proveedor de seminarios web a través del paso de flujo [!UICONTROL Cambiar estado del programa] cuando el [!UICONTROL Nuevo estado] se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, realice el paso de flujo [!UICONTROL Cambiar estado del programa] #1 y el paso de flujo [!UICONTROL Enviar correo electrónico] #2.

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
