---
unique-page-id: 1146980
description: 'Uso de Añadir opción en un paso de flujo: Documentos de Marketo: Documentación del producto'
title: Uso de la opción Añadir en un paso de flujo
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Uso de la opción Añadir en un paso de flujo {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

**Agregar opción** permite utilizar un paso de flujo y decir &quot;Depende&quot; al elegir los detalles.

1. En el **Flujo** de la campaña inteligente, añada cualquier paso de flujo y haga clic en **Agregar opción**.

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. Seleccione la condición de opción.

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. Elija el operador de opciones e introduzca un valor de opción. Esto establece sus criterios o opciones.

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. Introduzca un valor de paso de flujo para la opción.

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >Tokens **not** trabajar en la parte de condición de un paso de flujo de opciones.

1. Repita los pasos anteriores para agregar varias opciones y, a continuación, agregue o ajuste el valor predeterminado.

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >Puede establecer cualquiera de sus pasos de flujo en —No hacer nada—, en cuyo caso no se realizará ninguna acción sobre esa elección.

   >[!CAUTION]
   >
   >Solo se aplica la primera opción coincidente al paso de flujo. Obtenga información sobre cómo  [reordenar &quot;Agregar opción&quot; en una acción de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md).

   ¡Excelente! Ahora puede crear una sola campaña inteligente con opciones de paso de flujo en lugar de crear varias campañas inteligentes para cada opción.

   >[!MORELIKETHIS]
   >
   >[Reordenar la opción Añadir opción en un paso de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md)
