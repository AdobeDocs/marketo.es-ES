---
unique-page-id: 2949874
description: 'Creación de un evento con el seminario web de Goto: documentos de Marketo, documentación del producto'
title: Crear un evento con el seminario web de Goto
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Crear un evento con el seminario web de Goto {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Agregar el seminario web GoToWebinar como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Establezca las [acciones de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)adecuadas para rastrear la participación

Cree primero su seminario web en GoToWebinar. Algunos ajustes en la creación de su GoToWebinar los utiliza Marketo y otros solo los utiliza GoToWebinar.

Después de crear un evento de Marketo y asociar el seminario web de GoTo con él, los sistemas podrán compartir la información de registro y asistencia.

A continuación se muestra una lista de las configuraciones utilizadas por Marketo.

## Título y descripción {#title-and-description}

**Nombre del seminario web** - escriba el nombre para el seminario web. Este nombre se puede ver en Marketo.

**Descripción** (opcional): escriba la descripción del seminario web. La descripción se puede ver en Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Fecha y hora {#date-time}

Introduzca la siguiente información para el seminario web y se incorporará a Marketo mediante el adaptador. Si realiza cambios en esta información, debe hacer clic en el vínculo &quot;**Actualizar del proveedor de seminarios web**&quot; en **Acciones de eventos** para que Marketo vea los cambios.

**Fecha de inicio** - escribe tu fecha de inicio. Esto se puede ver en Marketo.

**Hora de inicio** - ingrese su hora de inicio. Esto se puede ver en Marketo.

**Hora de finalización**: introduzca la hora de finalización. Esto se puede ver en Marketo.

**Zona horaria**: seleccione la zona horaria aplicable. Se puede ver en Marketo.

**Tipo -** establecido en **Una sesión**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Actualmente, Marketo no admite seminarios web recurrentes. Debe configurar una sola sesión entre cada evento de Marketo y seminario web de GoTo.

>[!TIP]
>
>Si necesita ayuda adicional para el seminario web de GoToWebinar, visite su [Sitio de ayuda](https://support.logmeininc.com/gotowebinar).

Ahora, ¡vamos a saltar a Marketo!

1. Seleccione un evento. Haga clic en **Acciones de eventos** y elija **Configuración de eventos**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario web**.

1. Elija **GoToWebinar** de la lista de **socios de evento**.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Elija la cuenta.

   ![](assets/rtaimage-2.png)

1. Seleccione el seminario web.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. ¡Excelente! Ahora **GoToWebinar** sincroniza y programa el evento.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellidos, Dirección de correo electrónico. Estos campos son obligatorios y no deben estar vacíos.

   >[!TIP]
   >
   >Para rellenar el correo electrónico de confirmación con esta dirección URL única, use el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
   >
   >Establece tu correo electrónico de confirmación en **Operativo** para asegurarte de que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de tanto tiempo aún no ves nada, selecciona **Actualizar del proveedor de seminarios web** en el menú Acciones de eventos en la pestaña **Resumen** de tu evento.

Las personas que se suscriban a su seminario web se transferirán al proveedor del seminario web a través del paso de flujo Cambiar estado del programa cuando el nuevo estado se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de realizar los pasos de flujo Cambiar estado del programa #1 y Enviar correo electrónico #2.

## Visualización de la programación  {#viewing-the-schedule}

En la vista de programación, haga clic en la entrada de calendario del evento. Puede ver la programación en la parte derecha de la pantalla.

>[!NOTE]
>
>Para cambiar la programación del evento, tendrá que editar el seminario web en GoToWebinar.

![](assets/image2015-5-14-15-3a3-3a13.png)
