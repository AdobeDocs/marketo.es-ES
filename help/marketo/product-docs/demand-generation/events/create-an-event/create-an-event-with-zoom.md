---
unique-page-id: 17728023
description: Crear un evento con  [!DNL Zoom] - Documentos de Marketo - Documentación del producto
title: Crear un evento con  [!DNL Zoom]
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Crear un evento con [!DNL Zoom] {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Agregar [!DNL Zoom] como [!DNL LaunchPoint] servicio](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Establezca las [acciones de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) apropiadas para rastrear la participación

Primero cree su seminario web en [!DNL Zoom]. Marketo utiliza ciertas opciones de configuración en la creación de su [!DNL Zoom], y algunas solo las usa [!DNL Zoom].

Después de crear un evento de Marketo y asociarle un seminario web de [!DNL Zoom], los sistemas podrán compartir la información de registro y asistencia. Para obtener ayuda para crear un seminario web, consulte [Introducción a  [!DNL Zoom] Seminarios web](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Introduzca la siguiente información para el seminario web y se incorporará a Marketo mediante el adaptador. Si realiza cambios en esta información, debe hacer clic en el vínculo &quot;Actualizar desde el proveedor de seminarios web&quot; en Acciones de eventos para que Marketo vea los cambios.

**Título y descripción**

* **Nombre del seminario web**: escriba el nombre del seminario web. Este nombre se puede ver en Marketo.

* **Descripción** (opcional): escriba la descripción del seminario web. La descripción se puede ver en Marketo.

**Fecha y hora**

* **Fecha de inicio** - Escriba la fecha de inicio. Esto se puede ver en Marketo.

* **Hora de inicio** - Escriba la hora de inicio. Esto se puede ver en Marketo.

* **Duración**: escriba la duración. La hora de inicio y la hora de finalización se podrán ver en Marketo.

* **Zona horaria**: seleccione la zona horaria aplicable. Esto se puede ver en Marketo.

* **Seminario web recurrente**: no marcar.

* **Registro**: marque esta casilla para que el registro sea obligatorio. Utilizará un formulario o una página de aterrizaje de Marketo para capturar la información de registro que se insertará en [!DNL Zoom].

>[!NOTE]
>
>Actualmente, Marketo no admite seminarios web recurrentes. Debe configurar una sola sesión entre cada evento de Marketo y [!DNL Zoom] seminario web.

![](assets/overview2.png)

>[!TIP]
>
>Hay campos adicionales que configurará en [!DNL Zoom] que NO afectarán la integración. Consulta el [[!DNL Zoom] Centro de ayuda para seminarios web](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) para obtener más información sobre estos campos.

Ahora, ¡vamos a saltar a Marketo!

1. Seleccione un evento. Haga clic en **[!UICONTROL Acciones de eventos]** y elija **[!UICONTROL Configuración de eventos]**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario web**.

1. Elija **[!UICONTROL Zoom]** de la lista de **[!UICONTROL Socios de eventos]**.

   ![](assets/eventsettings1.png)

1. Elija la cuenta [!DNL Zoom] con la que desea asociar el evento.

   ![](assets/selectaccount.png)

1. Seleccione el seminario web.

   ![](assets/selectevent.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/eventsettingssave.png)

   ¡Excelente! Ahora [!DNL Zoom] sincroniza y programa el evento.

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellidos, Dirección de correo electrónico.

   >[!TIP]
   >
   >Para rellenar el correo electrónico de confirmación con esta dirección URL única, use el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
   >
   >Establece tu correo electrónico de confirmación en **Operativo** para asegurarte de que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

   Las personas que se suscriban a tu seminario web se transferirán a tu proveedor de seminarios web a través del paso de flujo **[!UICONTROL Cambiar estado del programa]** cuando el [!UICONTROL Nuevo estado] se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de hacer que el paso de flujo **[!UICONTROL Cambiar estado del programa]** #1 y el paso de flujo **[!UICONTROL Enviar correo electrónico]** #2.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de tanto tiempo aún no ves nada, selecciona **Actualizar del proveedor de seminarios web** en el menú Acciones de eventos en la pestaña **Resumen** de tu evento y luego haz clic en el icono de actualización en la parte inferior derecha de la pantalla.
