---
unique-page-id: 2949863
description: 'Creación de un evento con Webex: documentos de Marketo, documentación del producto'
title: Creación de un evento con Webex
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Creación de un evento con Webex {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Añadir Webex como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Configure las variables apropiadas [acciones de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) para rastrear la participación
>* Asegúrese de utilizar Eventos Webex (clásico)

Cree primero un evento Webex en el Centro de eventos Webex. Marketo solo utiliza configuraciones y campos específicos para su integración, que se explicarán en breve. Otros campos que puede que desee configurar para Webex se explican en la sección [Guía del usuario del centro de eventos Webex](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>Marketo Engage solo admite eventos creados en Eventos Webex (clásico). Marketo no admite eventos creados en Eventos Webex (nuevos) en este momento.

## Información básica {#basic-information}

* **Nombre del evento -** Este nombre se puede ver en Marketo.
* **Casilla de verificación No incluida**

   * Se recomienda que lo haga **no** enumere su evento. Esto garantizará que todas las personas se registren a través de su página de aterrizaje de Marketo. Las personas que se registren mediante un mecanismo que no sea Marketo se mostrarán en Marketo una vez finalizado el evento Y solo si han asistido al evento.
   * Si elige enumerar el evento, aparecerá en la página Lista de eventos para todas las personas que visiten el sitio web del Centro de eventos.

* **Registro -** Marque esta casilla para establecer como &quot;obligatorio&quot;. Utilizará un formulario o una página de aterrizaje de Marketo para capturar información de registro que se insertará en Webex.
* **Contraseña de evento**- (opcional) Si utiliza este campo, asegúrese de incluirlo en su correo electrónico de confirmación.

![](assets/image2015-5-28-13-3a30-3a55.png)

## Fecha y hora {#date-time}

* **Fecha de inicio** - Introduzca la fecha de inicio. Esto se puede ver en Marketo.

* **Hora de inicio** - Introduzca la hora de inicio. Esto se puede ver en Marketo.

* **Duración estimada** - Especifique la duración del evento. Esto se puede ver en Marketo.

* **Zonas horarias** : introduzca las zonas horarias aplicables. Se pueden ver en Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Configuración de audioconferencia {#audio-conference-settings}

Esta configuración solo reside en Webex. No los utiliza ni los puede ver en Marketo, pero pueden ser importantes para el seminario web, por lo que vuelva a comprobarlos.

## Descripción y opciones del evento  {#event-description-options}

Las siguientes opciones las utiliza o puede ver en Marketo. Otros campos solo residen en Webex.

* **Descripción** - Introduzca una descripción. Esto será visible, pero no modificable, en Marketo.
* **Encuesta posterior al evento** : Marketo no puede capturar la información en una encuesta posterior al evento de Webex en este momento.
* **URL de destino** : (opcional) puede introducir la dirección URL de una página de aterrizaje de Marketo para que sirva como dirección URL de destino que se mostrará después de que finalice la sesión.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Asistentes y registro {#attendees-registration}

Controlará la lista de invitaciones, el formulario de registro y otros correos electrónicos mediante un evento de Marketo. Marketo no admitirá otras funciones, como:

* **Número máximo de solicitantes de registro** - Actualmente **no** compatible mediante la integración Marketo-Webex.  La aprobación manual de los solicitantes de registro está disponible mediante el estado de progresión Pendiente de aprobación en Marketo.

* **Se requiere ID de registro** - Actualmente compatible con la integración Marketo-Webex. Puede utilizar Marketo para enviar el correo electrónico de confirmación del evento. Cuando la persona se registra, recibe una dirección URL única que utiliza para entrar en el evento.

  >[!TIP]
  >
  >Para rellenar el correo electrónico de confirmación con esta dirección URL única, utilice el siguiente token en el correo electrónico: `{{member.webinar url}}`. Cuando se envía la dirección URL de confirmación, este token se resuelve automáticamente en la dirección URL de confirmación única de la persona.
  >
  >Defina su correo electrónico de confirmación en **Operativo** para garantizar que las personas que se registren y puedan darse de baja sigan recibiendo su información de confirmación.

* **Contraseña de registro** - (Opcional) Actualmente no es compatible con la integración Marketo-Webex.
* **Reglas de aprobación** - Actualmente no es compatible con la integración Marketo-Webex. Sin embargo, puede utilizar campañas inteligentes en Marketo para controlar las aprobaciones.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Presentadores y panelistas {#presenters-panelists}

La información configurada en esta sección no se pasa a Marketo.

### Mensajes de correo electrónico {#email-messages}

Utilizará Marketo para enviar correos electrónicos a sus registrantes, correos electrónicos de confirmación, etc. No es necesario configurar nada en esta sección. Desactive las opciones de mensajes de correo electrónico en Webex.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>La integración Marketo-Webex no puede admitir el envío de correos electrónicos de confirmación desde Webex. La confirmación debe enviarse a través de Marketo. Una vez programado el evento, asegúrese de copiar la información del evento en el correo electrónico de confirmación de Marketo y establecer el correo electrónico como **Operativo**.

¡Ahora estamos listos para saltar a Marketo!

1. Seleccione el evento que ha creado. Abra el **Acciones de evento** menú desplegable. Elegir **Configuración de eventos.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario web**.

1. En **Socio de evento**, seleccione **Webex**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. En **Iniciar sesión**, elija su inicio de sesión en Webex.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. En **Evento**, elija el evento Webex recién creado. A continuación, seleccione una página de copia de seguridad opcional y haga clic en **Guardar**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Seleccione una página de respaldo opcional para su evento Webex. Elija en el menú desplegable de páginas de aterrizaje de Marketo aprobadas o introduzca la URL de una página de aterrizaje que no sea de Marketo.

   >[!TIP]
   >
   >Configure una página de copia de seguridad para dirigir a un miembro a una página específica si hace clic en la URL de su evento personalizado antes de la hora de inicio del evento.

   >[!NOTE]
   >
   >Los campos que Marketo envía son: Nombre, Apellidos, Dirección de correo electrónico.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos, como se muestra arriba.

   >[!TIP]
   >
   >Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de esperar tanto tiempo aún no ve nada, seleccione **Actualizar del proveedor de seminarios web** en el menú Acciones de evento de **Resumen** de su evento.

¡Dulce! El evento Webex ahora se sincroniza con el evento Marketo. Las personas que se suscriban a su seminario web se transferirán al proveedor del seminario web a través del paso de flujo Cambiar estado del programa cuando el nuevo estado se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Además, asegúrese de realizar los pasos de flujo Cambiar estado del programa #1 y Enviar correo electrónico #2.

## Visualización de la programación  {#viewing-the-schedule}

En la vista de programación, haga clic en la entrada de calendario del evento. Puede ver la programación en la parte derecha de la pantalla.

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Para cambiar la programación del evento, tendrá que editar el seminario web en Webex.
