---
unique-page-id: 17728023
description: 'Creación de un evento con Zoom: Documentos de Marketo, documentación del producto'
title: Creación de un evento con zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Creación de un evento con zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Añadir Zoom como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Configure las variables apropiadas [acciones de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)para rastrear la participación

Primero cree su seminario web en Zoom. Marketo utiliza ciertos ajustes en la creación del Zoom y algunos solo los utiliza Zoom.

Después de crear un evento de Marketo y asociar un seminario web de Zoom con él, los sistemas podrán compartir la información de registro y asistencia. Para obtener ayuda con la creación de un seminario web, consulte  [Introducción a los seminarios web de Zoom](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Introduzca la siguiente información para el seminario web y se incorporará a Marketo mediante el adaptador. Si realiza cambios en esta información, debe hacer clic en el vínculo &quot;Actualizar desde el proveedor de seminarios web&quot; en Acciones de eventos para que Marketo vea los cambios.

**Título y descripción**

* **Nombre del seminario web** : introduzca el nombre del seminario web. Este nombre se puede ver en Marketo.

* **Descripción** (opcional): escriba la descripción del seminario web. La descripción se puede ver en Marketo.

**Fecha y hora**

* **Fecha de inicio** - Introduzca la fecha de inicio. Esto se puede ver en Marketo.

* **Hora de inicio** - Introduzca la hora de inicio. Esto se puede ver en Marketo.

* **Duración** : introduzca la duración. La hora de inicio y la hora de finalización se podrán ver en Marketo.

* **Zona horaria** - Seleccione la zona horaria aplicable. Esto se puede ver en Marketo.

* **Seminario web recurrente**- Manténgase sin marcar.

* **Registro** - Marque esta casilla para que el registro sea obligatorio. Utilizará un formulario o una página de aterrizaje de Marketo para capturar la información de registro que se insertará en Zoom.

>[!NOTE]
>
>Actualmente, Marketo no admite seminarios web recurrentes. Debe configurar una sola sesión entre cada seminario web de Marketo Event y Zoom.

![](assets/overview2.png)

>[!TIP]
>
>Hay campos adicionales que configurará en Zoom que NO afectarán a la integración. Consulte la [Centro de ayuda del seminario web Zoom](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) para obtener más información sobre estos campos.

Ahora, ¡vamos a saltar a Marketo!

1. Seleccione un evento. Clic **Acciones de evento** y elija **Configuración de eventos**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario web**.

1. Elegir **Zoom** desde el **Evento** **Socio** Lista.

   ![](assets/eventsettings1.png)

1. Elija la cuenta de Zoom con la que desea asociar el evento.

   ![](assets/selectaccount.png)

1. Seleccione el seminario web.

   ![](assets/selectevent.png)

1. Clic **Guardar**.

   ![](assets/eventsettingssave.png)

   ¡Excelente! Ahora Zoom sincroniza y programa el evento.

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellidos, Dirección de correo electrónico.

   >[!TIP]
   >
   >Para rellenar el correo electrónico de confirmación con esta dirección URL única, utilice el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
   >
   >Defina su correo electrónico de confirmación en **Operativo** para garantizar que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

   Las personas que se suscriban a su seminario web se enviarán al proveedor del seminario web a través del **Cambiar estado del programa** Paso de flujo cuando el Nuevo estado se establece en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de hacer **Cambiar estado del programa** paso de flujo #1, y **Enviar correo electrónico** paso de flujo #2.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar del proveedor de seminarios web** en el menú Acciones de evento de **Resumen** de su evento.
