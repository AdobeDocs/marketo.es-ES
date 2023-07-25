---
unique-page-id: 1146997
description: 'Uso de un token de fecha en un paso de flujo de espera: documentos de Marketo, documentación del producto'
title: Uso de un token de fecha en un paso de flujo de espera
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Uso de un token de fecha en un paso de flujo de espera {#use-a-date-token-in-a-wait-flow-step}

Puede utilizar el paso Flujo de espera para pausar el recorrido de una persona a través de una campaña inteligente hasta una fecha en particular que utilice un token de fecha. También puede modificar la fecha de finalización en un número determinado de días.

>[!NOTE]
>
>Esto solo se aplica a las campañas de déclencheur. No puede utilizar esta función en campañas por lotes.

1. En su campaña inteligente **Flujo** , arrastre el cursor sobre la pestaña **Esperar** paso de flujo.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Haga clic en el icono de engranaje a la derecha.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Desde el **Tipo** menú desplegable, seleccione **Token de fecha**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Elija un token de fecha para especificar cuándo debe finalizar el paso de espera:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Para esperar hasta el siguiente aniversario de la fecha del año natural actual o siguiente, marque la casilla.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilice esta opción en tokens de fecha que hagan referencia a fechas del pasado, como un cumpleaños o una fecha de inicio del contrato.

1. De forma opcional, puede modificar la fecha de finalización un número determinado de días.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >También puede especificar el número de días mediante una `{{lead.` o `{{company.` token que representa un campo entero o un `{{my.` token de tipo numérico.

1. Clic **Guardar**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Utilizar una duración en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
