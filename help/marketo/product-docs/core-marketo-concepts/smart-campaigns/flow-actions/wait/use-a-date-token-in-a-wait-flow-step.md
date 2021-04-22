---
unique-page-id: 1146997
description: 'Uso de un token de fecha en un paso de flujo de espera: Documentos de Marketo: Documentación del producto'
title: Uso de un token de fecha en un paso de flujo de espera
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Utilizar un token de fecha en un paso de flujo de espera {#use-a-date-token-in-a-wait-flow-step}

Puede utilizar el paso Flujo de espera para pausar el recorrido de una persona a través de una campaña inteligente hasta una fecha concreta que utilice un token de fecha. También puede modificar la fecha de finalización en un número de días.

>[!NOTE]
>
>Esto solo se aplica a las campañas de déclencheur. No puede utilizar esta función en campañas por lotes.

1. En la pestaña **Flow** de la campaña inteligente, arrastre el paso de flujo **Wait**.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Haga clic en el icono del engranaje a la derecha.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. En la lista desplegable **Type**, seleccione **Date Token**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Elija un token de fecha para especificar cuándo debe finalizar el paso de espera:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Para esperar hasta el próximo aniversario de la fecha que se produzca en el año natural actual o siguiente, marque la casilla .

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilice esta opción en los tokens de fecha que hacen referencia a fechas anteriores, como cumpleaños o fecha de inicio del contrato.

1. De forma opcional, puede modificar la fecha de finalización en un número específico de días.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >También puede especificar el número de días utilizando un token `{{lead.` o `{{company.` que representa un campo entero o un token `{{my.` del tipo numérico.

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Usar una duración en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

