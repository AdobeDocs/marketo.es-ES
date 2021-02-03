---
unique-page-id: 2949874
description: Crear un Evento con GotoWebinar - Documentos de marketing - Documentación del producto
title: Crear un Evento con el seminario web GotoWebinar
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---


# Crear un Evento con GotoWebinar {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Añadir GoToWebinar como un servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Crear un nuevo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Configure las [acciones de flujo adecuadas](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)para rastrear la participación


Primero cree su seminario web en GoToWebinar. Marketo utiliza ciertos ajustes en la creación de su GoToWebinar y algunos solo los utiliza GoToWebinar.

Después de crear un evento de marketing y asociar el GoToWebinar con él, los sistemas podrán compartir la información de registro y asistencia.

A continuación se muestra una lista de la configuración utilizada por Marketing.

## Título y descripción {#title-and-description}

**Nombre**  del seminario web: introduzca el nombre del seminario web. Este nombre se podrá ver en Marketing.

**Descripción**  (opcional): introduzca la descripción del seminario web. La descripción será`visible en Marketing.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Fecha y hora {#date-time}

Introduzca la siguiente información para el seminario web y se colocará en el equipo de marketing a través del adaptador. Si realiza cambios en esta información, debe hacer clic en el vínculo &quot;**Actualizar desde el proveedor de seminario web**&quot; en **Acciones de Evento**, para que Marketing pueda ver los cambios.

**Fecha**  de inicio: introduzca la fecha de inicio. Esto se podrá ver en Marketing.

**Hora**  del inicio: introduzca la hora del inicio. Esto se podrá ver en Marketing.

**Hora**  de finalización: introduzca la hora de finalización. Esto se podrá ver en Marketing.

**Huso horario** : seleccione el huso horario correspondiente. Será visible en Marketing.

**Escriba -** establecido en  **Una sesión**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Actualmente, Marketing no admite seminarios Web recurrentes. Debe configurar una sola sesión entre cada Evento de marketing y el seminario web de GoToWebinar.

>[!TIP]
>
>Si necesita ayuda adicional de GoToWebinar, visite su [sitio de ayuda](https://support.logmeininc.com/gotowebinar).

Ahora, ¡saltemos al mercado!

1. Seleccione un evento. Haga clic en **Acciones de Evento** y elija **Configuración de Evento**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario web**.

1. Elija **GoToWebinar** en la Lista **Socio de Evento**.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Elija la cuenta.

   ![](assets/rtaimage-2.png)

1. Seleccione el seminario web.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Haga clic en **Guardar**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. ¡Excelente! Ahora el evento está sincronizado y programado por **GoToWebinar**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Los campos que envía Marketing to son: Nombre, Apellido, Dirección De Correo Electrónico. Estos campos son obligatorios y no deben estar vacíos.

   >[!TIP]
   >
   >Para completar el correo electrónico de confirmación con esta dirección URL única, utilice el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
   >
   >Configure el correo electrónico de confirmación en **Operativo** para asegurarse de que las personas que se registren y puedan cancelarse la suscripción sigan recibiendo la información de confirmación.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar sus correos electrónicos de confirmación. Utilice la campaña inteligente del programa de evento en su lugar, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketing. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar desde el proveedor de seminario web** en el menú Acciones de Evento de la ficha **Resumen** del evento.

Las personas que se registren en el seminario web se enviarán a su proveedor de seminarios web a través del paso Cambiar el estado del Programa cuando el estado nuevo se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de que el paso 1 del flujo de cambio de estado de Programa y el paso 2 del flujo de envío de correo electrónico.

## Visualización del programa {#viewing-the-schedule}

En la vista calandario del programa, haga clic en la entrada de calendario del evento. Puede ver la programación en el lado derecho de la pantalla.

>[!NOTE]
>
>Para cambiar el programa de evento, deberá editar el seminario web en GoToWebinar.

![](assets/image2015-5-14-15-3a3-3a13.png)
