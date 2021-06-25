---
unique-page-id: 17728023
description: 'Creación de un evento con zoom: documentos de Marketo: documentación del producto'
title: Crear un evento con zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Crear un evento con zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Agregar zoom como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
* Configure las [acciones de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)adecuadas para rastrear la participación


Primero cree su seminario web en Zoom. Marketo utiliza ciertos ajustes en la creación del zoom y algunos solo lo hacen con el zoom.

Después de crear un evento de Marketo y asociar un seminario web de Zoom con él, los sistemas podrán compartir la información de registro y asistencia. Para obtener ayuda sobre la creación de un seminario web, consulte [Introducción a los seminarios web de zoom](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Introduzca la siguiente información para su seminario web y se extraerá en Marketo a través del adaptador. Si realiza algún cambio en esta información, debe hacer clic en el vínculo &quot;Actualizar desde el proveedor de seminarios web&quot; en Acciones de evento, para que Marketo pueda ver los cambios.

**Título y descripción**

* **Nombre del seminario web** : introduzca el nombre del seminario web. Este nombre se puede ver en Marketo.

* **Descripción**  (opcional): introduzca la descripción del seminario web. La descripción se puede ver en Marketo.

**Fecha y hora**

* **Fecha de inicio** : introduzca la fecha de inicio. Esto se puede ver en Marketo.

* **Hora de inicio** : introduzca la hora de inicio. Esto se puede ver en Marketo.

* **Duración** : introduzca la duración. La hora de inicio y de finalización se pueden ver en Marketo.

* **Zona horaria** : seleccione la zona horaria correspondiente. Esto se puede ver en Marketo.

* **Seminario web recurrente**: Manténgase sin marcar.

* **Registro** : Marque esta casilla para que el registro sea necesario. Utilizará un formulario o una página de aterrizaje de Marketo para capturar la información de registro que se insertará en Zoom.

>[!NOTE]
Actualmente, Marketo no admite seminarios web recurrentes. Debe configurar una sola sesión entre cada seminario web Evento de Marketo y Zoom.

![](assets/overview2.png)

>[!TIP]
Hay campos adicionales que puede configurar en Zoom que NO afectarán a la integración. Consulte el [Centro de ayuda del seminario web de zoom](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) para obtener más información sobre estos campos.

¡Ahora vamos a entrar en Marketo!

1. Seleccione un evento. Haga clic en **Acciones de evento** y elija **Configuración de evento**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   El tipo de canal del evento seleccionado debe ser **webinar**.

1. Elija **Zoom** en la lista **Evento** **Socio**.

   ![](assets/eventsettings1.png)

1. Elija la cuenta de zoom con la que desee asociar el evento.

   ![](assets/selectaccount.png)

1. Seleccione el seminario web.

   ![](assets/selectevent.png)

1. Haga clic en **Guardar**.

   ![](assets/eventsettingssave.png)

   ¡Excelente! Ahora el evento se sincroniza y programa mediante el zoom.

   >[!NOTE]
   Los campos que Marketo envía son: Nombre, Apellido, Dirección De Correo Electrónico.

   >[!TIP]
   Para rellenar el correo electrónico de confirmación con esta dirección URL única, utilice el token siguiente en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
   Configure el correo electrónico de confirmación en **Operativo** para asegurarse de que las personas que se registren y puedan darse de baja reciban la información de confirmación.

   Las personas que se registren en el seminario web se enviarán al proveedor de seminarios web a través del paso de flujo **Cambiar estado del programa** cuando el nuevo estado esté configurado como &quot;Registrado&quot;. Ningún otro estado empuja a la persona. Además, asegúrese de realizar **Change Program Status** paso de flujo #1 y **Send Email** paso de flujo #2.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar desde el proveedor de seminarios web** en el menú Acciones de evento de la pestaña **Resumen** del evento.
