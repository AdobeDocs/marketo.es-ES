---
unique-page-id: 2949863
description: Crear un Evento con WebEx - Documentos de marketing - Documentación del producto
title: Crear un Evento con WebEx
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---


# Crear un Evento con WebEx {#create-an-event-with-webex}

>[!NOTE]
>
>**Requisitos previos**
>
>* [Añadir WebEx como un servicio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Crear un nuevo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Configure las acciones de [flujo adecuadas para](http://docs.marketo.com/display/DOCS/Flow+Actions)realizar el seguimiento de la participación


Primero cree un Evento Webex en el Centro de Evento WebEx. Marketo utiliza únicamente la configuración y los campos específicos para su integración, que se completarán en breve. Otros campos que puede que desee configurar para WebEx se explican en la Guía [del usuario de](http://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf)WebEx Evento Center.

## Información básica {#basic-information}

* **Nombre de evento: este nombre se podrá ver en Marketing** .
* **Casilla de verificación no enumerada**

   * Se recomienda que **no haga** listas en su evento. Esto garantizará que todas las personas se registren a través de la página de aterrizaje de marketing. Las personas que se registren a través de un mecanismo que no sea Marketing se mostrarán en Marketing después de que el evento haya finalizado Y sólo si asistieron al evento.
   * Si elige la lista del evento, aparecerá en la página Lista de Eventos para cualquiera que visite el sitio web del Centro de Evento.

* **Registro -** Marque esta casilla para establecer en &quot;requerido&quot;. Utilizará un formulario o una página de aterrizaje de marketing para capturar la información de registro que se insertará en WebEx.
* **Contraseña** de evento: (opcional) si utiliza este campo, asegúrese de incluirlo en su correo electrónico de confirmación.

![](assets/image2015-5-28-13-3a30-3a55.png)

## Fecha y hora {#date-time}

* **Fecha** de inicio: introduzca la fecha de inicio. Esto se podrá ver en Marketing.

* **Hora** de inicio: Introduzca la hora de inicio. Esto se podrá ver en Marketing.

* **Duración** estimada: especifique la duración del evento. Esto se podrá ver en Marketing.

* **Husos horarios** : introduzca los husos horarios aplicables. Serán visibles en Marketing.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Ajustes de conferencia de audio {#audio-conference-settings}

Esta configuración solo reside en WebEx. No son usadas por o visibles en Marketing, pero pueden ser importantes para su seminario web, por lo que los dobles de revisión!

## Descripción y opciones de evento  {#event-description-options}

Las siguientes opciones son usadas por o visibles en Marketing. Otros campos solo residen en WebEx.

* **Descripción** : introduzca una descripción. Esto será visible pero no modificable en Marketing.
* **Encuesta** posterior al evento: Marketo no puede capturar la información en una encuesta posterior al evento WebEx en este momento.
* **Dirección URL** de destino: (opcional) puede introducir la dirección URL de una página de aterrizaje de marketing para que sirva de dirección URL de destino que se mostrará una vez finalizada la sesión.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Asistentes y registro {#attendees-registration}

Controlará la lista de invitación, el formulario de registro y otros correos electrónicos mediante un Evento de marketing. Marketo no admitirá otras funciones, entre las que se incluyen:

* **Número máximo de usuarios registrados** : actualmente **no** se admite con la integración de Marketing a WebEx.  La aprobación manual de los usuarios registrados está disponible mediante el estado de progresión Pendiente de aprobación en Marketing.

* **ID de registro requerido** : admitido actualmente mediante la integración de Marketing-WebEx. Puede utilizar Marketo para enviar el correo electrónico de confirmación de su evento. Cuando la persona se registra, recibe una dirección URL única que utiliza para entrar en el evento.

   >[!TIP]
   >
   >Para completar el correo electrónico de confirmación con esta dirección URL única, utilice el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
   >
   >Configure el correo electrónico de confirmación en **Operativo** para asegurarse de que las personas que se registren y puedan cancelarse la suscripción sigan recibiendo la información de confirmación.

* **Contraseña** de registro: (opcional) actualmente no se admite con la integración de Marketing a WebEx.
* **Reglas** de aprobación: Actualmente no se admite con la integración de Marketing a WebEx. Sin embargo, puede utilizar campañas inteligentes en Marketing para controlar las aprobaciones.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Presentadores y panelistas {#presenters-panelists}

La información configurada en esta sección no se pasa a Marketing.

### Mensajes de correo electrónico {#email-messages}

Usará Marketo para enviar correos electrónicos a sus usuarios registrados, correos electrónicos de confirmación, etc. No necesita configurar nada en esta sección. Desactive (desmarque) las opciones de mensajes de correo electrónico en WebEx.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>La integración de Marketing-WebEx no admite el envío de correos electrónicos de confirmación desde WebEx. La confirmación debe enviarse a través de Marketing. Después de programar el evento, asegúrese de copiar la información del evento en el correo electrónico de confirmación de marketing y establecer el correo electrónico como **operativo**.

¡Ahora estamos listos para saltar al mercado!

1. Seleccione el evento que ha creado. Abra la lista desplegable Acciones **de** Evento. Elija Configuración **de Evento.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario** web.

1. En Socio **de** Evento, seleccione **WebEx**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. En **Inicio de sesión**, elija el inicio de sesión de WebEx.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. En **Evento**, elija el evento WebEx recién creado. A continuación, seleccione una página de copia de seguridad opcional y haga clic en **Guardar**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Seleccione una página de respaldo opcional para su evento WebEx. Elija una de las opciones de la lista desplegable de páginas de aterrizaje de marketing aprobadas o introduzca la dirección URL de una página de aterrizaje que no sea de marketing.

   >[!TIP]
   >
   >Configure una página de copia de seguridad para dirigir a un miembro a una página específica si hace clic en la URL de evento personalizada antes de la hora de inicio del evento.

   >[!NOTE]
   >
   >Los campos que envía Marketing to son: Nombre, Apellido, Dirección De Correo Electrónico.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar sus correos electrónicos de confirmación. Utilice la campaña inteligente del programa de evento en su lugar, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketing. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar desde el proveedor** de seminario web en el menú Acciones de Evento de la ficha **Resumen** de su evento.

¡Dulce! El evento de WebEx ahora se sincroniza con el evento de marketing.  Las personas que se registren en el seminario web se enviarán a su proveedor de seminarios web a través del paso Cambiar el estado del Programa cuando el estado nuevo se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de que el paso 1 del flujo de cambio de estado de Programa y el paso 2 del flujo de envío de correo electrónico.

## Visualización de la programación  {#viewing-the-schedule}

En la vista [de](http://docs.marketo.com/display/docs/program+schedule+view)calandario del programa, haga clic en la entrada de calendario del evento. Puedes ver la programación en el lado derecho de la pantalla!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Para cambiar la programación de eventos, deberá editar el seminario web en WebEx.
