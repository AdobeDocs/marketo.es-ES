---
unique-page-id: 2949865
description: Crear un Evento con Adobe Connect - Documentos de marketing - Documentación del producto
title: Creación de un Evento con Adobe Connect
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# Crear un Evento con Adobe Connect {#create-an-event-with-adobe-connect}

La sincronización con Adobe Connect le permite administrar el registro y la asistencia a los seminarios web dentro de Marketing, lo que garantiza que la participación no se desplace.

>[!PREREQUISITES]
>
>* [Vincular Adobe Connect y Marketing](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Crear un nuevo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


En primer lugar, asegúrese de haber creado la reunión o el seminario en Adobe Connect. Si necesita ayuda, consulte la [Guía del usuario de Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html). Las reuniones y los seminarios que cree en Adobe Connect deben crearse en la carpeta especificada al introducir sus credenciales en Marketing. Después de crear la reunión o el seminario, tenga en cuenta cualquier información logística relevante (como el número de teléfono), para utilizarla en el correo electrónico de confirmación y en el archivo ICS.

>[!NOTE]
>
>En este momento **no** admitimos Adobe Connect On-Site.

1. En el inicio de un nuevo evento, seleccione **Acciones de Evento** y, a continuación, **Configuración de Evento**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Si no ve **Configuración de Evento** en la lista desplegable, asegúrese de que el canal del evento tenga **Evento con el seminario web** seleccionado en &quot;Se aplica a&quot;.

1. En **Socio de Evento**, seleccione **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Seleccione su **Id. de inicio de sesión** y seleccione su **Evento**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Haga clic en **Guardar**.

   ![](assets/event-settings-overview.png)

   ¡Bonito! El evento de Adobe Connect ahora se sincroniza con el evento de marketing.

   >[!NOTE]
   >
   >Los campos que envía Marketing to son: Nombre, Apellido, Dirección De Correo Electrónico.

   >[!TIP]
   >
   >Para insertar la dirección URL única de la persona en un correo electrónico, utilice este token: `{{member.webinar url}}`. Cuando se envía el correo electrónico, este token resuelve automáticamente la dirección URL de confirmación única de la persona desde Adobe Connect.
   >
   >Configure el correo electrónico de confirmación en **Operativo** para asegurarse de que las personas que se registren y puedan cancelarse la suscripción sigan recibiendo la información de confirmación.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar sus correos electrónicos de confirmación. Utilice la campaña inteligente del programa de evento en su lugar, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketing. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar desde el proveedor de seminario web** en el menú Acciones de Evento de la ficha Resumen del evento.

   >[!MORELIKETHIS]
   >
   > * [Añadir Adobe Connect como un servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   > * [Editar un Canal de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)


Las personas que se registren en el seminario web se enviarán a su proveedor de seminarios web a través del paso Cambiar el estado del Programa cuando el estado nuevo se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de que el paso 1 del flujo de cambio de estado de Programa y el paso 2 del flujo de envío de correo electrónico.
