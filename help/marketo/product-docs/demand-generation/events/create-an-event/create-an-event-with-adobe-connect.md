---
unique-page-id: 2949865
description: 'Creación de un evento con Adobe Connect: documentos de Marketo, documentación del producto'
title: Creación de un evento con Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '419'
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
>Como host de evento, asegúrese de unirse desde la aplicación y **no** mediante el vínculo enviado a los asistentes.

>[!NOTE]
>
>En este momento no se admite Adobe Connect en el sitio.

1. En la página principal de un nuevo evento, seleccione **Acciones de evento**, y luego **Configuración de eventos**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Si no lo ve... **Configuración de eventos** en la lista desplegable, asegúrese de que el canal del evento tenga **Evento con seminario web** seleccionados en &quot;Se aplica a&quot;.

1. En **Socio de evento**, seleccione **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Seleccione su **Iniciar sesión** ID y seleccione su **Evento**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Clic **Guardar**.

   ![](assets/event-settings-overview.png)

   ¡Bonito! El evento de Adobe Connect ahora se sincroniza con el evento de Marketo.

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellidos, Dirección de correo electrónico.

   >[!TIP]
   >
   >Para insertar la URL única de la persona en un correo electrónico, utilice este token: `{{member.webinar url}}`. Cuando se envía el correo electrónico, este token resuelve automáticamente la URL de confirmación única de la persona desde Adobe Connect.
   >
   >Defina su correo electrónico de confirmación en **Operativo** para garantizar que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

   Las personas que se suscriban a su seminario web se transferirán al proveedor del seminario web a través del paso de flujo Cambiar estado del programa cuando el nuevo estado se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de realizar los pasos de flujo Cambiar estado del programa #1 y Enviar correo electrónico #2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar del proveedor de seminarios web** en el menú Acciones de evento de la pestaña Resumen del evento.

   >[!MORELIKETHIS]
   >
   >* [Añadir Adobe Connect as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Editar un canal de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
