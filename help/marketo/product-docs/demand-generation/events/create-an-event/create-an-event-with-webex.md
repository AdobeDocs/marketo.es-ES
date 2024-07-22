---
unique-page-id: 2949863
description: 'Creación de un evento con Webex: documentos de Marketo, documentación del producto'
title: Creación de un evento con Webex
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Creación de un evento con Webex {#create-an-event-with-webex}

Después de crear un seminario web en Webex, deberá sincronizar el evento con Marketo Engage.

>[!PREREQUISITES]
>
>* [Agregar Webex como servicio de LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Crear un nuevo programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Establezca las [acciones de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) apropiadas para rastrear la participación

## Programar el seminario web {#schedule-your-webinar}

Programas tu evento y eliges tu configuración preferida en [Webex](https://www.webex.com/){target="_blank"}. Solo puede verse la siguiente información en Marketo: nombre del seminario web, fecha y hora de inicio y finalización, zona horaria y descripción. Encontrará información adicional sobre los seminarios web de Webex [aquí](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

### Información básica {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **Tema**: Este es su nombre de evento y se podrá ver en Marketo.
* **Fecha y hora**: La fecha de inicio y finalización, la hora de inicio y finalización, la duración y la zona horaria son visibles en Marketo.
* **Máximo de asistentes**: El número máximo de asistentes determina qué características de Webex son compatibles.
* **Vista de webcast para asistentes**: Marque esta opción para que su seminario web se transmita en vivo a todos los asistentes.
* **Panelistas**: Invita a personas específicas a ser panelistas en tu seminario web.
* **Agenda del seminario web**: rellene esta sección si desea proporcionar contexto en la invitación por correo electrónico que se envía a los panelistas.

### Seguridad {#security}

![](assets/create-an-event-with-webex-2.png)

* **Contraseña del seminario web**: (opcional) Si utiliza este campo, asegúrese de incluirlo en el correo electrónico de confirmación.
* **Contraseña para la lista de paneles**: (opcional) Si utiliza este campo, asegúrese de incluirlo en la agenda del seminario web.
* **Requerir cuenta**: limita a los asistentes únicamente a aquellos que tienen cuentas de Webex.

### Opciones de conexión de audio {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Tipo de conexión de audio**: elige cómo los participantes del seminario web se unen a la parte de audio del seminario web.
* **Tono de entrada y salida**: seleccione el sonido que desee que emitan los usuarios cuando alguien entre o salga del seminario web (se requiere conexión de audio telefónica).
* **Silenciar lista de paneles**: elija la configuración de Silenciar lista de paneles que desee.

### Opciones avanzadas {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Grabación automática**: Marque esta opción para que su seminario web se registre automáticamente.
* **Sesión de práctica**: Marque esta opción para que se inicie una sesión de práctica cuando comience el seminario web.
* **Sesiones de desglose**: Las sesiones de desglose le permiten preasignar panelistas y asistentes antes de que comience el seminario web o permitirles unirse durante este.
* **Serie de seminarios web**: agregar a una serie de seminarios web permite que los usuarios vean el seminario web, sea público o no.
* **Registro**: Requiere que los asistentes se registren y reciban la aprobación del host antes de asistir.
* **Recordatorio por correo electrónico**: elige un recordatorio por correo electrónico que vaya desde 15 minutos antes de que el seminario web comience hasta dos días.
* **Opciones de seminario web**: determina qué características están disponibles para los participantes en el seminario web.
* **Privilegios de participante**: Los privilegios de participante determinan las acciones disponibles para los participantes del seminario web.

>[!NOTE]
>
>La integración Marketo-Webex no puede admitir el envío de correos electrónicos de confirmación desde Webex. La confirmación debe enviarse a través de Marketo. Después de programar el evento, asegúrese de copiar la información del evento en el correo electrónico de confirmación de Marketo y establecer el correo electrónico como _Operativo_.

## Sincronizar el evento con el Marketo Engage {#sync-your-event-with-marketo-engage}

1. En Marketo, busque y seleccione el programa de eventos deseado. En la lista desplegable **Acciones de eventos**, seleccione **Configuración de eventos**.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >El tipo de canal del evento seleccionado debe ser **seminario web**.

1. En el menú desplegable **Socio de evento**, seleccione **Seminarios web de Webex**.

   ![](assets/create-an-event-with-webex-6.png)

1. En el menú desplegable **Iniciar sesión**, elija el inicio de sesión de Webex.

   ![](assets/create-an-event-with-webex-7.png)

1. En el menú desplegable **Evento**, elige tu evento Webex.

   ![](assets/create-an-event-with-webex-8.png)

1. Se rellenarán los detalles del seminario web. Haga clic en **Guardar**.

   ![](assets/create-an-event-with-webex-9.png)

El evento de Webex ahora se sincroniza con el programa de eventos de Marketo. Las personas que se suscriban a tu seminario web se transferirán a tu proveedor de seminarios web a través del paso de flujo _Cambiar estado del programa_ cuando el nuevo estado se establezca en &quot;Registrado&quot;. Ningún otro estado empujará a la persona. Asegúrese de hacer que el paso de flujo _Cambiar estado del programa_ #1 y el paso de flujo _Enviar correo electrónico_ #2.

## Cosas que hay que tener en cuenta {#things-to-note}

* Evite utilizar programas de correo electrónico anidados para enviar los correos electrónicos de confirmación. En su lugar, utilice la campaña inteligente del programa de eventos.

* Los datos pueden tardar hasta 48 horas en aparecer en Marketo. Si después de tanto tiempo aún no ves nada, haz clic en **Actualizar del proveedor de seminarios web** en la lista desplegable **Acciones de eventos** en la pestaña **Resumen** de tu programa de eventos.
