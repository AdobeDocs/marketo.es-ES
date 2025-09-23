---
unique-page-id: 1146997
description: 'Uso de un token de fecha en un paso de flujo de espera: documentos de Marketo, documentación del producto'
title: Uso de un token de fecha en un paso de flujo de espera
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 9%

---

# Uso de un token de fecha en un paso de flujo de espera {#use-a-date-token-in-a-wait-flow-step}

Puede utilizar el paso Flujo de espera para pausar el recorrido de una persona a través de una campaña inteligente hasta una fecha concreta que utilice un token de fecha. También puede modificar la fecha de finalización en un número determinado de días.

>[!NOTE]
>
>Esto solo se aplica a las campañas de Déclencheur. No puede utilizar esta función en campañas por lotes.

1. En la pestaña **[!UICONTROL Flujo]** de tu campaña inteligente, arrastra el cursor sobre el paso de flujo **[!UICONTROL Esperar]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. Haga clic en el icono de engranaje.

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. En el menú desplegable **[!UICONTROL Tipo]**, seleccione **[!UICONTROL Token de fecha]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. Elija un [!UICONTROL Token de fecha] para especificar cuándo debe finalizar el paso de espera:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. Para esperar hasta el siguiente aniversario de la fecha del año natural actual o siguiente, marque la casilla.

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >Utilice esta opción en tokens de fecha que hagan referencia a fechas del pasado, como un cumpleaños o una fecha de inicio del contrato.

1. De forma opcional, puede modificar la fecha de finalización un número determinado de días.

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >También puede especificar el número de días utilizando un token `{{lead.` o `{{company.` que represente un campo entero o un token `{{my.` de tipo numérico.

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [Usar una duración en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
