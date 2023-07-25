---
unique-page-id: 1146978
description: 'Uso de una duración en un paso de flujo de espera: documentos de Marketo, documentación del producto'
title: Utilizar una duración en un paso de flujo de espera
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Utilizar una duración en un paso de flujo de espera {#use-a-duration-in-a-wait-flow-step}

Puede utilizar el paso Flujo de espera para pausar el recorrido de una persona a través de una campaña inteligente durante un tiempo determinado. También puede especificar criterios para el día de la semana y la hora en que termina.

1. En su campaña inteligente **Flujo** , arrastre el cursor sobre la pestaña **Esperar** paso de flujo.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Escriba el tiempo que desea pausar.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. ¡Eso es todo! El flujo se pausará durante la duración especificada. Para obtener opciones avanzadas, haga clic en el icono de engranaje a la derecha.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Especifique el día de la semana en el que debe finalizar el paso de espera.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Si lo desea, especifique la hora. Clic **Guardar**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Una persona déclencheur una campaña inteligente el viernes a las 5 p. m. El paso de espera es avanzado: 48 horas y debe finalizar el lunes a viernes a las 9 a. m.
   >
   >El resultado sería que la persona continuaría en el flujo el **Lunes, 9 a. m**. Esta es la primera cita M-F después de 48 horas.

   >[!NOTE]
   >
   >La duración, las fechas, las horas y los días utilizados dependen del huso horario de la suscripción.

   >[!MORELIKETHIS]
   >
   >* [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [Uso de un token de fecha en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
