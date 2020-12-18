---
unique-page-id: 10096679
description: Ejemplo de integración de Evento ON24 - Documentos de marketing - Documentación del producto
title: Ejemplo de integración de Evento ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Ejemplo de integración de Evento ON24 {#example-on-event-integration}

Aquí hay un evento de muestra, incluyendo campañas, para un seminario web sobre el 24 de octubre. Cuando cree el evento, asegúrese de probar las campañas antes de ejecutarlas.

## Crear un nuevo Evento en Actividades de marketing {#create-a-new-event-in-marketing-activities}

1. Seleccione **Nuevo** > **Nuevo Programa**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Seleccione una **carpeta de Campaña** en la que se alojará el evento.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Escriba un **Nombre** para el evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Seleccione **Evento **como **Tipo de Programa**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Seleccione **Seminario web **como **Canal **para el evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Haga clic en **Crear**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invitar (Campaña por lotes) {#invite-batch-campaign}

* **Lista**  inteligente: defina a quién va a invitar al evento.
* **Flujo**

   * Enviar correo electrónico: si se trata de un correo electrónico de recurso local, tendrá la siguiente convención de nombre: EventName.EmailName. También puede utilizar correos electrónicos globales.
   * Cambiar estado en progresión: defina en Seminario web > Invitado.

* **Programación** : establezca la fecha de envío de la invitación.

## Registro/Confirmación (Campaña desencadenadora) {#registration-confirmation-trigger-campaign}

* **Lista inteligente**

   * Active la campaña en función de **Rellena el formulario**. Asegúrese de incluir la página de aterrizaje en la que se encuentra el formulario mediante **Añadir restricción**, especialmente si el formulario se utiliza en varias páginas de aterrizaje.

>[!CAUTION]
>
>Debe utilizar un formulario de marketing para registrar personas para el evento o un formulario que no sea de marketing con la integración de API adecuada para insertar los datos de registro en Marketing. Esto es fundamental para el éxito de la integración de socios de Evento. **NOTA**: Si está utilizando un formulario de Marketo en una página de aterrizaje que no sea de Marketo, el activador será  **Rellenar** formulario con el nombre del formulario.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flujo**

   * **Cambiar estado en progresión** : defina en Seminario web > Registrado. **PRECAUCIÓN**: Este paso de flujo es necesario al configurar la campaña secundaria. Cuando el estado de progresión de una persona cambia a **Registrado**, Marketing coloca la información de registro en ON24.

   * **Enviar correo electrónico** : mensaje de correo electrónico de confirmación (configurado en  **** Operationstambién que las personas que se han registrado aún lo reciben).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTA**: Si la persona es devuelta con un error de registro, no recibirá la confirmación por correo electrónico.

## Recordatorio (Campaña por lotes) {#reminder-batch-campaign}

* **Lista**  inteligente: filtre mediante  **Miembro de** programación y defina el estado como  **Registrado**.

* **Flujo** : enviar correo electrónico (correo electrónico recordatorio).

**NOTA**: Podría usar una campaña similar para enviar un correo electrónico de seguimiento  ** diferente a las personas invitadas pero que aún no se han registrado.

## Campaña de seguimiento (Campaña por lotes o desencadenador) {#follow-up-campaign-batch-or-trigger-campaign}

* **Lista**  inteligente: activador basado en cambios en el estado del programa.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flujo** : enviar correo electrónico. Utilice las opciones para enviar distintos correos electrónicos en función del estado del programa.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>* [Explicación de los Eventos del adaptador de Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



