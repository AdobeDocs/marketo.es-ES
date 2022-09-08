---
unique-page-id: 10096679
description: Ejemplo de integración de eventos ON24 - Documentos de Marketo - Documentación del producto
title: Ejemplo de integración de eventos ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Ejemplo de integración de eventos ON24 {#example-on-event-integration}

>[!IMPORTANT]
>
>A partir de agosto de 2022, ON24 ya no es compatible con las nuevas integraciones de Marketo. La información de este artículo solo se aplica a los usuarios existentes.

Este es un evento de ejemplo, incluidas campañas, para un seminario web sobre ON24. Al crear el evento, asegúrese de probar las campañas antes de ejecutarlas.

## Crear un nuevo evento en actividades de marketing {#create-a-new-event-in-marketing-activities}

1. Select **Nuevo** > **Nuevo programa**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Seleccione un **Carpeta de campaña** donde se activará el evento.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Escriba un **Nombre** para el evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Select **Evento** como el **Tipo de programa**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Select **Seminario web** como el **Canal** para el evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Haga clic en **Crear**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invitar (campaña por lotes)  {#invite-batch-campaign}

* **Lista inteligente** - Defina a quién invitará al evento.
* **Flujo**

   * Enviar correo electrónico : si se trata de un correo electrónico de recurso local, tendrá la siguiente convención de nombres: EventName.EmailName. También puede utilizar correos electrónicos globales.
   * Cambio de estado en progresión: establezca en Seminario web > Invitado.

* **Programación** - Defina la fecha de envío de la invitación.

## Registro/Confirmación (Campaña de Déclencheur) {#registration-confirmation-trigger-campaign}

* **Lista inteligente**

   * Déclencheur de la campaña en función de **Rellena el formulario**. Asegúrese de incluir la página de aterrizaje en la que se encuentra el formulario mediante **Agregar restricción**, especialmente si el formulario se utiliza en varias páginas de aterrizaje.

>[!CAUTION]
>
>Debe utilizar un formulario de Marketo para registrar personas para el evento o un formulario que no sea de Marketo con la integración API adecuada para insertar los datos de registro en Marketo. Esto es fundamental para el éxito de la integración de socios de evento. **NOTA**: Si utiliza un formulario de Marketo en una página de aterrizaje que no sea de Marketo, el déclencheur será **Rellena el formulario** con el nombre del formulario.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flujo**

   * **Cambiar estado en progresión** - Configúrelo en Seminario web > Registrado. **PRECAUCIÓN**: Este paso de flujo es necesario al configurar la campaña secundaria. Cuando el estado de progresión de una persona cambia a **Registrados**, Marketo envía la información de registro a ON24.

   * **Enviar correo electrónico** - Correo electrónico de confirmación (establecido en **Operativo** para que las personas que se han registrado aún lo reciban).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTA**: Si la persona es devuelta con un error de registro, no recibirá la confirmación por correo electrónico.

## Recordatorio (campaña por lotes) {#reminder-batch-campaign}

* **Lista inteligente** - Filtrar usando **Miembro del Programa** y establezca el estado en **Registrados**.

* **Flujo** - Enviar correo electrónico (correo electrónico recordatorio).

**NOTA**: Puede utilizar una campaña similar para enviar una *different* correo electrónico de seguimiento a las personas invitadas pero que aún no se han registrado.

## Campaña de seguimiento (campaña por lotes o de Déclencheur) {#follow-up-campaign-batch-or-trigger-campaign}

* **Lista inteligente** - Déclencheur basado en cambios en el estado del programa.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flujo** - Enviar correo electrónico. Utilice las opciones para enviar diferentes correos electrónicos en función del estado del programa.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
