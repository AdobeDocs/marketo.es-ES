---
unique-page-id: 10096677
description: Probar la integración de eventos ON24 - Documentos de Marketo - Documentación del producto
title: Probar la integración de eventos ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Probar la integración de eventos ON24 {#test-your-on-event-integration}

Asegúrese de probar la integración del evento exhaustivamente.

## Secuencia de prueba recomendada antes de ejecutar la primera campaña {#recommended-test-sequence-before-running-your-first-campaign}

1. Complete el formulario de registro del evento y utilice una dirección de correo electrónico válida para probar.
1. Confirme que el nombre de la prueba se muestra con un **Registrados** en la cuadrícula Pertenencia del evento de Marketo.
1. Confirme que el nombre de la prueba también se muestra como **Registrados** en ON24.
1. Confirme que la dirección de correo electrónico válida que utilizó para registrar el nombre de prueba recibió un correo electrónico de confirmación al evento y que la dirección URL única se resolvió en el correo electrónico.

   >[!NOTE]
   >
   >Debe usar la variable `{{member.webinar url}}` en el correo electrónico de confirmación para que se muestre la dirección URL única en el correo electrónico de cada registrador.

## Después del evento {#after-the-event}

Así es como se actualizan los datos después de que se produzca el evento:

* Marketo recupera todos los días los datos de los asistentes de ON24.
* Una vez que los datos de los asistentes se sincronizan entre Marketo y ON24, Marketo actualiza el estado de pertenencia a Asistido, Asistido bajo demanda o Sin programa. En la variable **Resumen** , el estado del evento se actualiza a **Finalización del evento**.

>[!MORELIKETHIS]
>
>* [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
>* [Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}

