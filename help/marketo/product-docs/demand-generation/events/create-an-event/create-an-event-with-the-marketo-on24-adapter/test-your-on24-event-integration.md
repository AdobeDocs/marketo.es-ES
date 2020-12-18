---
unique-page-id: 10096677
description: Probar la integración del Evento ON24 - Documentos de marketing - Documentación del producto
title: Probar la integración del Evento ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Probar la integración del Evento ON24 {#test-your-on-event-integration}

Asegúrese de probar la integración de evento a fondo.

## Secuencia de prueba recomendada antes de ejecutar la primera Campaña {#recommended-test-sequence-before-running-your-first-campaign}

1. Rellene el formulario de registro del evento y utilice una dirección de correo electrónico válida para realizar la prueba.
1. Confirme que el nombre de la prueba se muestra con un estado **Registrado** en la cuadrícula Membresía del evento de marketing.
1. Confirme que el nombre de la prueba también se muestra como **Registrado** en ON24.
1. Confirme que la dirección de correo electrónico válida que utilizó para registrar el nombre de prueba recibió un correo electrónico de confirmación al Evento y que la dirección URL única se resolvió en el mensaje de correo electrónico.

   >[!NOTE]
   >
   >Debe utilizar el token `{{member.webinar url}}` en el correo electrónico de confirmación para que la dirección URL única se muestre en el correo electrónico de cada registrado.

## Después del Evento {#after-the-event}

A continuación se muestra cómo se actualizan los datos después de que se produzca el evento:

* Marketo recupera los datos de los asistentes de ON24 cada noche.
* Una vez que los datos del asistente se sincronizan entre Marketo y ON24, Marketo actualiza el estado de pertenencia a Asistentes, Asistentes a petición o Sin mostrar. En la ficha **Resumen** del evento, el estado del evento se actualiza a **Evento completado**.

>[!MORELIKETHIS]
>
>* [Ejemplo de integración de Evento ON24](example-on24-event-integration.md)
>* [Explicación de los Eventos del adaptador de Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



