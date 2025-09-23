---
unique-page-id: 1146980
description: 'Uso de Agregar opción en un paso de flujo: documentos de Marketo, documentación del producto'
title: Uso de Añadir opción en un paso de flujo
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 7%

---

# Uso de Añadir opción en un paso de flujo {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Agregar un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

&quot;Agregar opción&quot; le permite utilizar un paso de flujo y decir &quot;depende&quot; al elegir los detalles.

1. En la ficha **[!UICONTROL Flujo]** de la campaña inteligente, agregue cualquier paso de flujo y haga clic en **[!UICONTROL Agregar opción]**.

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. Seleccione la condición de elección.

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. Seleccione el operador de opción e introduzca un valor de opción. Esto establece los criterios de selección.

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. Introduzca un valor de paso de flujo para la opción.

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >Los tokens _no_ funcionarán en la condición como parte de un paso del flujo de opciones.

1. Repita los pasos anteriores para agregar varias opciones y, a continuación, agregue o ajuste el valor predeterminado.

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >Puede establecer cualquiera de los pasos de flujo en —Do Nothing—, en cuyo caso no se llevará a cabo ninguna acción sobre esa opción.

   >[!CAUTION]
   >
   >Solo se aplica la primera opción coincidente al paso de flujo. Aprenda a [reordenar &quot;Agregar opción&quot; en una acción de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   ¡Excelente! Ahora puede crear una sola campaña inteligente con opciones de paso de flujo en lugar de crear varias campañas inteligentes para cada opción.

   >[!MORELIKETHIS]
   >
   >[Reordenar la opción de adición en un paso de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
