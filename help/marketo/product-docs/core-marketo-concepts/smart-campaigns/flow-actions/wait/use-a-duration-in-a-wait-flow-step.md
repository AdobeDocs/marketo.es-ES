---
unique-page-id: 1146978
description: Aprenda a utilizar una duración en un paso de flujo de espera. Pausar el flujo durante un número determinado de días antes de la siguiente acción.
title: Utilizar una duración en un paso de flujo de espera
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/4T2sVyYvhrxdvwELe0DXw0zvGCywwHDKAuDGlIiIN9Q
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 216
ht-degree: 8%

---

# Utilizar una duración en un paso de flujo de espera {#use-a-duration-in-a-wait-flow-step}

Puede utilizar el paso Flujo de espera para pausar el recorrido de una persona a través de una campaña inteligente durante un tiempo determinado. También puede especificar criterios para el día de la semana y la hora en que termina.

1. En la pestaña **[!UICONTROL Flujo]** de tu campaña inteligente, arrastra el cursor sobre el paso de flujo **[!UICONTROL Esperar]**.

   ![](assets/use-a-duration-in-a-wait-flow-step-1.png)

1. Escriba el tiempo que desea pausar.

   ![](assets/use-a-duration-in-a-wait-flow-step-2.png)

1. El flujo se pausa durante la duración especificada. Para obtener opciones avanzadas, haga clic en el icono de engranaje a la derecha.

   ![](assets/use-a-duration-in-a-wait-flow-step-3.png)

1. Especifique el día de la semana en el que debe finalizar el paso de espera.

   ![](assets/use-a-duration-in-a-wait-flow-step-4.png)

1. Si lo desea, especifique la hora. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/use-a-duration-in-a-wait-flow-step-5.png)

   >[!NOTE]
   >
   >**Ejemplo**
   >
   >Una persona déclencheur una campaña inteligente el viernes a las 5 p. m. El paso de espera es avanzado: 48 horas y debe finalizar el lunes a viernes a las 9 a. m.
   >
   >El resultado sería que la persona continuaría en el flujo el **lunes a las 9 a. m.**. Esta es la primera cita M-F después de 48 horas.

   >[!NOTE]
   >
   >La duración, las fechas, las horas y los días utilizados dependen del huso horario de la suscripción.

   >[!MORELIKETHIS]
   >
   >* [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [Usar un token de fecha en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
