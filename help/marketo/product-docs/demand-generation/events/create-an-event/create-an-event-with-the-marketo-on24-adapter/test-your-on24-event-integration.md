---
unique-page-id: 10096677
description: Prueba de la integración de eventos ON24 - Documentos de Marketo - Documentación del producto
title: Prueba de la integración de eventos ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Prueba de la integración de eventos ON24 {#test-your-on-event-integration}

Asegúrese de probar exhaustivamente la integración de eventos.

## Secuencia De Prueba Recomendada Antes De Ejecutar La Primera Campaña {#recommended-test-sequence-before-running-your-first-campaign}

1. Rellene el formulario de registro del evento y utilice una dirección de correo electrónico válida para realizar la prueba.
1. Confirme que el nombre de la prueba se muestra con un estado **Registrado** en la cuadrícula Pertenencia de su evento de Marketo.
1. Confirme que el nombre de la prueba también se muestra como **Registrado** en ON24.
1. Confirme que la dirección de correo electrónico válida que utilizó para registrar el nombre de la prueba recibió un correo electrónico de confirmación al evento y que la dirección URL única se resuelve en el correo electrónico.

   >[!NOTE]
   >
   >Debe utilizar el token `{{member.webinar url}}` en el correo electrónico de confirmación para que se muestre la dirección URL única en el correo electrónico de cada solicitante de registro.

## Después del evento {#after-the-event}

Así se actualizan los datos después de que tenga lugar el evento:

* Marketo recupera los datos de los asistentes de ON24 todas las noches.
* Una vez que los datos de los asistentes se sincronizan entre Marketo y ON24, Marketo actualiza el estado de pertenencia a [!UICONTROL Asistido], [!UICONTROL Asistido a petición] o [!UICONTROL Sin presentación]. En la ficha **[!UICONTROL Resumen]** del evento, el estado del evento se actualiza a **[!UICONTROL Evento completado]**.

>[!MORELIKETHIS]
>
>* [Ejemplo de integración de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
