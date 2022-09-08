---
unique-page-id: 10096677
description: Probar la integración de eventos ON24 - Documentos de Marketo - Documentación del producto
title: Probar la integración de eventos ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Probar la integración de eventos ON24 {#test-your-on-event-integration}

>[!IMPORTANT]
>
>A partir de agosto de 2022, ON24 ya no es compatible con las nuevas integraciones de Marketo. La información de este artículo solo se aplica a los usuarios existentes.

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
>* [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

