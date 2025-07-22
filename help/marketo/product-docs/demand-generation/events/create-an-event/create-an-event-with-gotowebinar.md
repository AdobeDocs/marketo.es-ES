---
unique-page-id: 2949874
description: Crear un evento con  [!DNL GotoWebinar] - Documentos de Marketo - Documentación del producto
title: Crear un evento con  [!DNL GotoWebinar]
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Crear un evento con [!DNL GotoWebinar] {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Agregar [!DNL GoToWebinar] como [!DNL LaunchPoint] servicio](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Establezca las [acciones de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) apropiadas para rastrear la participación

Primero cree su seminario web en [!DNL GoToWebinar]. Marketo utiliza ciertas opciones de configuración en la creación de su [!DNL GoToWebinar], y algunas solo las usa [!DNL GoToWebinar].

Después de crear un evento de Marketo y asociar [!DNL GoToWebinar] con él, los sistemas podrán compartir la información de registro y asistencia.

A continuación se muestra una lista de las configuraciones utilizadas por Marketo.

## Título y descripción {#title-and-description}

**[!UICONTROL Título]** - escriba el nombre para el seminario web. Este nombre se puede ver en Marketo.

**[!UICONTROL Descripción]** (opcional): escriba la descripción del seminario web. La descripción se puede ver en Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Fecha y hora {#date-time}

Introduzca la siguiente información para el seminario web y se incorporará a Marketo mediante el adaptador. Si realiza cambios en esta información, debe hacer clic en el vínculo &quot;**[!UICONTROL Actualizar del proveedor de seminarios web]**&quot; en **[!UICONTROL Acciones de eventos]** para que Marketo vea los cambios.

**[!UICONTROL Fecha de inicio]** - ingrese la fecha de inicio. Esto se puede ver en Marketo.

**[!UICONTROL Hora de inicio]** - ingrese su hora de inicio. Esto se puede ver en Marketo.

**[!UICONTROL Hora de finalización]**: introduzca la hora de finalización. Esto se puede ver en Marketo.

**[!UICONTROL Zona horaria del seminario web]**: seleccione la zona horaria aplicable. Se puede ver en Marketo.

**[!UICONTROL Tipo]** - establecido en **[!UICONTROL Una sesión]**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Actualmente, Marketo no admite seminarios web recurrentes. Debe configurar una sola sesión entre cada evento de Marketo y [!DNL GoToWebinar] seminario web.

>[!TIP]
>
>Si necesita ayuda adicional de [!DNL GoToWebinar], visite su [Sitio de ayuda](https://support.logmeininc.com/gotowebinar).

Ahora, ¡vamos a saltar a Marketo!

1. Seleccione un evento. Haga clic en **[!UICONTROL Acciones de eventos]** y elija **[!UICONTROL Configuración de eventos]**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario web**.

1. Elija **[!UICONTROL GoToWebinar]** de la lista de **[!UICONTROL socios de evento]**.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Elija la cuenta.

   ![](assets/rtaimage-2.png)

1. Seleccione el seminario web.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. ¡Excelente! Ahora **[!DNL GoToWebinar]** sincroniza y programa el evento.

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
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de tanto tiempo aún no ves nada, selecciona **[!UICONTROL Actualizar del proveedor de seminarios web]** en el menú [!UICONTROL Acciones de eventos] de la pestaña **[!UICONTROL Resumen]** de tu evento.

Las personas que se suscriban a tu seminario web se transferirán a tu proveedor de seminarios web a través del paso de flujo [!UICONTROL Cambiar estado del programa] cuando el [!UICONTROL Nuevo estado] se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de hacer que el paso de flujo [!UICONTROL Cambiar estado del programa] #1 y el paso de flujo [!UICONTROL Enviar correo electrónico] #2.

## Visualización de la programación  {#viewing-the-schedule}

En la vista de programación, haga clic en la entrada de calendario del evento. Puede ver la programación en la parte derecha de la pantalla.

>[!NOTE]
>
>Para cambiar la programación de eventos, tendrá que editar el seminario web del [!DNL GoToWebinar].

![](assets/image2015-5-14-15-3a3-3a13.png)
