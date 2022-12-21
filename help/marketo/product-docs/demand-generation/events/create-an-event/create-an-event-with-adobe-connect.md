---
unique-page-id: 2949865
description: 'Creación de un evento con Adobe Connect: Marketo Docs: documentación del producto'
title: Creación de un evento con Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Creación de un evento con Adobe Connect {#create-an-event-with-adobe-connect}

La sincronización con Adobe Connect le permite administrar el registro y la asistencia a los seminarios web dentro de Marketo, lo que garantiza que la participación no se desplace.

>[!PREREQUISITES]
>
>* [Vincular Adobe Connect y Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


En primer lugar, asegúrese de haber creado la reunión o el seminario en Adobe Connect. Si necesita ayuda, consulte la [Guía del usuario de Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Las reuniones y seminarios que cree en Adobe Connect deben crearse en la carpeta que especificó al introducir sus credenciales en Marketo. Después de crear la reunión o el seminario, tome nota de cualquier información logística relevante (como el número de teléfono) que pueda utilizar en el correo electrónico de confirmación y en el archivo ICS.

>[!CAUTION]
>
>Como host de eventos, asegúrese de unirse desde la aplicación y **not** mediante el vínculo enviado a los asistentes.

>[!NOTE]
>
>En este momento no se admite Adobe Connect On-Site.

1. En la página principal de un nuevo evento, seleccione **Acciones de evento** y luego **Configuración de eventos**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Si no ve **Configuración de eventos** en la lista desplegable , asegúrese de que el canal del evento tenga **Evento con seminario web** seleccionado en &quot;Se aplica a&quot;.

1. En **Socio de evento**, seleccione **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Seleccione su **Inicio de sesión** ID y seleccione su **Evento**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Haga clic en **Guardar**.

   ![](assets/event-settings-overview.png)

   ¡Muy bien! El evento de Adobe Connect ahora se sincroniza con el evento de Marketo.

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellido, Dirección De Correo Electrónico.

   >[!TIP]
   >
   >Para insertar la URL única de la persona en un correo electrónico, utilice este token: `{{member.webinar url}}`. Cuando se envía el correo electrónico, este token resuelve automáticamente la URL de confirmación única de la persona desde Adobe Connect.
   >
   >Configure el correo electrónico de confirmación en **Operativo** para garantizar que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

   Las personas que se registren en el seminario web se enviarán al proveedor de seminarios web a través del paso Cambiar el estado del programa cuando el nuevo estado esté configurado como &quot;Registrado&quot;. Ningún otro estado empuja a la persona. Además, asegúrese de realizar el paso 1 del flujo de cambio de estado del programa y el paso 2 del flujo de envío de correo electrónico.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar desde el proveedor de seminarios web** en el menú Acciones de evento de la ficha Resumen del evento.

   >[!MORELIKETHIS]
   >
   >* [Añadir Adobe Connect como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Editar un canal de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

