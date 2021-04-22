---
unique-page-id: 1146978
description: 'Uso de una duración en un paso de flujo de espera: Documentos de Marketo: Documentación del producto'
title: Usar una duración en un paso de flujo de espera
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Usar una duración en un paso de flujo de espera {#use-a-duration-in-a-wait-flow-step}

Puede utilizar el paso Flujo de espera para pausar el recorrido de una persona a través de una campaña inteligente durante un tiempo determinado. También puede especificar criterios para el día de la semana y la hora en que finaliza.

1. En la pestaña **Flow** de la campaña inteligente, arrastre el paso de flujo **Wait**.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Escriba cuánto tiempo desea pausar.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. ¡Eso es todo! El flujo se detendrá durante el tiempo especificado. Para obtener opciones avanzadas, haga clic en el icono de engranaje a la derecha.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Especifique el día de la semana en el que debe finalizar el paso de espera.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Opcionalmente, especifique la hora. Haga clic en **Guardar**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Una persona déclencheur una campaña inteligente el viernes a las 5 pm. Se ha avanzado el paso de espera: 48 horas y debe terminar el lunes-viernes a las 9 de la mañana.
   >
   >El resultado sería que la persona continuaría en el flujo el **lunes a las 9 a. m.**. Esta es la primera fecha M-F después de 48 horas.

   >[!NOTE]
   >
   >La duración, las fechas, las horas y los días utilizados se basan en la zona horaria de la suscripción.

   >[!MORELIKETHIS]
   >
   >* [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [Uso de un token de fecha en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)

