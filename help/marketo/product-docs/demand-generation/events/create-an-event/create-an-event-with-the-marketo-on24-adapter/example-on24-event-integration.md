---
unique-page-id: 10096679
description: 'Ejemplo de integración de eventos ON24: Documentos de Marketo: documentación del producto'
title: Ejemplo de integración de eventos ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Ejemplo de integración de eventos ON24 {#example-on-event-integration}

Este es un evento de ejemplo, incluidas las campañas, para un seminario web ON24. Cuando cree su evento, asegúrese de probar las campañas antes de ejecutarlas.

## Crear un evento nuevo en actividades de marketing {#create-a-new-event-in-marketing-activities}

1. Seleccione **[!UICONTROL Nuevo]** > **[!UICONTROL Nuevo Programa]**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Seleccione una **[!UICONTROL carpeta de campañas]** en la que se activará el evento.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Escriba un **[!UICONTROL Nombre]** para el evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Seleccione **[!UICONTROL Evento]** como **[!UICONTROL Tipo de programa]**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Seleccione **[!UICONTROL Seminario web]** como **[!UICONTROL Canal]** para el evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invitar (campaña por lotes)  {#invite-batch-campaign}

* **Lista inteligente** - Define a quién invitarás al evento.
* **Flujo**

   * Enviar correo electrónico: si se trata de un correo electrónico de recurso local, tendrá la siguiente convención de nomenclatura: EventName.EmailName. También puede utilizar correos electrónicos globales.
   * Cambiar estado en progresión: establezca en Seminario web > Invitado.

* **Programación** - Establezca la fecha para enviar la invitación.

## Registro/Confirmación (Campaña de Déclencheur) {#registration-confirmation-trigger-campaign}

* **Lista inteligente**

   * Almacene en déclencheur la campaña según **[!UICONTROL Rellena el formulario]**. Asegúrese de incluir la página de aterrizaje en la que se encuentra el formulario mediante **[!UICONTROL Agregar restricción]**, especialmente si el formulario se utiliza en varias páginas de aterrizaje.

>[!CAUTION]
>
>Debe utilizar un formulario de Marketo para registrar a las personas en el evento o un formulario que no sea de Marketo con la integración de API adecuada para insertar los datos de registro en Marketo. Esto es fundamental para el éxito de su integración de [!UICONTROL Event Partner]. **NOTA**: Si está usando un formulario de Marketo en una página de aterrizaje que no sea de Marketo, su déclencheur será **[!UICONTROL Rellena el formulario]** con el [!UICONTROL Nombre del formulario].

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flujo**

   * **Cambiar estado en progresión** - Definir en Seminario web > Registrado. **PRECAUCIÓN**: Este paso de flujo es necesario al configurar su campaña secundaria. Cuando el estado de progresión de una persona cambia a **Registrada**, Marketo envía la información de registro a ON24.

   * **Enviar correo electrónico** - Correo electrónico de confirmación (configurado en **Operativo** para que las personas que cancelaron la suscripción y que se han registrado lo reciban).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTA**: Si la persona vuelve con un error de registro, no recibirá la confirmación por correo electrónico.

## Recordatorio (campaña por lotes) {#reminder-batch-campaign}

* **Lista inteligente** - Filtre con **Miembro del programa** y establezca el estado en **Registrado**.

* **Flujo** - Enviar correo electrónico (Correo electrónico de recordatorio).

**NOTA**: podrías usar una campaña similar para enviar un correo electrónico de seguimiento de *diferentes* a las personas invitadas pero que aún no se han registrado.

## Campaña de seguimiento (campaña por lotes o de Déclencheur) {#follow-up-campaign-batch-or-trigger-campaign}

* **Lista inteligente**: Déclencheur basado en los cambios en el estado del programa.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flujo** - Enviar correo electrónico. Utilice opciones para enviar diferentes correos electrónicos en función del estado del programa.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
