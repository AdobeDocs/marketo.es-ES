---
unique-page-id: 1146942
description: Definición de listas inteligentes para campañas inteligentes | Déclencheur - Documentos de Marketo - Documentación del producto
title: Definición de listas inteligentes para campañas inteligentes | DÉCLENCHEUR
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Definición de listas inteligentes para campañas inteligentes | DÉCLENCHEUR {#define-smart-list-for-smart-campaign-trigger}

Haga que una campaña inteligente se ejecute de a una persona a la vez en función de los eventos en directo mediante la adición de déclencheur.

1. En la campaña inteligente, haga clic en **Lista inteligente** pestaña.

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. Busque el déclencheur deseado y arrástrelo y suéltelo en el lienzo.

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >Se ejecuta una campaña inteligente con déclencheur en **Déclencheur** modo. Se ejecuta en una persona a la vez en función de los eventos activados y los filtros adicionales.

   >[!IMPORTANT]
   >
   >Cuando se utiliza un campo booleano en una lista inteligente de campañas de déclencheur, se debe establecer explícitamente en &quot;false&quot; para que el campo se evalúe correctamente durante la ejecución de la campaña.

1. Haga clic en la lista desplegable y seleccione un operador.

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >Las líneas rojas onduladas indican errores o falta información. Si no se corrige, la campaña no será válida y no se ejecutará.

   >[!TIP]
   >
   >En una campaña inteligente con déclencheur y filtros, los déclencheur se colocan en la parte superior y, cuando se activan, solo las personas que cumplen los criterios de filtro pasan por el flujo.

1. Defina el déclencheur.

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >Con varios déclencheur, una persona pasa por el flujo si **CUALQUIERA** se activa uno de los déclencheur.

Para ejecutar la campaña en un conjunto de personas al mismo tiempo, aprenda a [Definición de listas inteligentes para campañas inteligentes | Lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
