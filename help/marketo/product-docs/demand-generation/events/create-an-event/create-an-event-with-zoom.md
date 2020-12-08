---
unique-page-id: 17728023
description: Crear un Evento con zoom - Documentos de marketing - Documentación del producto
title: Creación de un Evento con zoom
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---


# Creación de un Evento con zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Añadir zoom como un servicio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Crear un nuevo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Configure las acciones de [flujo adecuadas para](http://docs.marketo.com/display/DOCS/Flow+Actions)realizar el seguimiento de la participación


Primero cree su seminario web en Zoom. Algunos ajustes de la creación del zoom son utilizados por Marketo y otros solo son utilizados por Zoom.

Después de crear un evento de marketing y asociar un seminario web de zoom con él, los sistemas podrán compartir la información de registro y asistencia. Para obtener ayuda sobre la creación de un seminario web, consulte [Introducción a los seminarios web](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)de zoom.

Introduzca la siguiente información para el seminario web y se colocará en el equipo de marketing a través del adaptador. Si realiza cambios en esta información, debe hacer clic en el vínculo &quot;Actualizar desde el proveedor de seminario web&quot; en Acciones de Evento, para que Marketing pueda ver los cambios.

**Título y descripción**

* **Nombre** del seminario web: introduzca el nombre del seminario web. Este nombre se podrá ver en Marketing.

* **Descripción** (opcional): introduzca la descripción del seminario web. La descripción será`visible en Marketing.

**Fecha y hora**

* **Fecha** de inicio: introduzca la fecha de inicio. Esto se podrá ver en Marketing.

* **Hora** de inicio: Introduzca la hora de inicio. Esto se podrá ver en Marketing.

* **Duración** : introduzca la duración. La hora de inicio y la hora de finalización se podrán ver en Marketing Cloud.

* **Huso horario** : seleccione el huso horario correspondiente. Esto se podrá ver en Marketing.

* **Seminario** web recurrente: no marcar.

* **Registro** : marque esta casilla para que el registro sea obligatorio. Utilizará un formulario o una página de aterrizaje de marketing para capturar la información de registro que se insertará en Zoom.

>[!NOTE]
>
>Actualmente, Marketing no admite seminarios Web recurrentes. Debe configurar una sola sesión entre cada Evento de marketing y cada seminario web de zoom.

![](assets/overview2.png)

>[!TIP]
>
>Hay campos adicionales que configurará en Zoom que NO afectarán a la integración. Consulte el Centro [de ayuda del seminario web de](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) zoom para obtener información adicional sobre estos campos.

Ahora, ¡saltemos al mercado!

1. Seleccione un evento. Haga clic en Acciones **de** Evento y elija Configuración **de Evento**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario** web.

1. Seleccione **Zoom** en la Lista **Evento** **Partner** .

   ![](assets/eventsettings1.png)

1. Elija la cuenta de zoom con la que desea asociar el evento.

   ![](assets/selectaccount.png)

1. Seleccione el seminario web.

   ![](assets/selectevent.png)

1. Haga clic en **Guardar**.

   ![](assets/eventsettingssave.png)

   ¡Excelente! Ahora el evento se sincroniza y programa mediante zoom.

   >[!NOTE]
   >
   >Los campos que envía Marketing to son: Nombre, Apellido, Dirección De Correo Electrónico.

   >[!TIP]
   >
   >Para completar el correo electrónico de confirmación con esta dirección URL única, utilice el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
   >
   >Configure el correo electrónico de confirmación en **Operativo** para asegurarse de que las personas que se registren y puedan cancelarse la suscripción sigan recibiendo la información de confirmación.

   Las personas que se registren en el seminario web se enviarán a su proveedor de seminarios web a través del paso de flujo **Cambiar estado** de Programa cuando el estado nuevo se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de realizar el paso 1 del flujo **Cambiar estado** de Programa y el paso 2 del flujo de **envío de correo electrónico** .

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar sus correos electrónicos de confirmación. Utilice la campaña inteligente del programa de evento en su lugar, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketing. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar desde el proveedor** de seminario web en el menú Acciones de Evento de la ficha **Resumen** de su evento.
