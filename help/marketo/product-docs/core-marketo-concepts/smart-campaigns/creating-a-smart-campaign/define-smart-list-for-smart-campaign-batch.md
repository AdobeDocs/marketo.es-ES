---
unique-page-id: 1146940
description: Definición de la lista inteligente para campañas inteligentes | Lote - Documentos de Marketo - Documentación del producto
title: Definición de la lista inteligente para campañas inteligentes | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 56d3d05d5462c79f32f507655266e3bfa0cc6846
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Definición de la lista inteligente para campañas inteligentes | Lote {#define-smart-list-for-smart-campaign-batch}

Las listas inteligentes son el mecanismo de Marketo para definir &quot;quién&quot; (qué personas) incluir, ya sea un informe, una lista o una campaña inteligente. A continuación se muestra cómo definir una lista inteligente para una campaña por lotes.

1. Elija una campaña inteligente y haga clic en **Lista inteligente**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Escriba para buscar un filtro y arrástrelo y suéltelo en el lienzo. Repita el proceso para varios filtros.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Una campaña inteligente con solo filtros se ejecuta en **Lote** en el menú contextual. Encuentra personas en la base de datos que califican según los filtros y los ejecuta a través del flujo a la vez.

   >[!NOTE]
   >
   >Puede hacer que una campaña inteligente se ejecute en una persona a la vez según los eventos en directo añadiendo déclencheur, lo que coloca la campaña inteligente en **Déclencheur** en el menú contextual.

1. Haga clic en la lista desplegable y elija un operador de filtro para el filtro que ha elegido.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Las líneas rojas indican errores o falta información. Si no se corrige, la campaña no será válida y no se ejecutará.

1. Introduzca el valor del filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >De forma predeterminada, se califican las personas que satisfacen TODAS las reglas de listas inteligentes. Esto se puede modificar para adaptarlo a sus necesidades de campaña. Consulte  [Reglas de lista inteligente para lógica compleja](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) para obtener más información.

   Para realizar déclencheur en eventos en directo de una persona a la vez, aprenda a [Definición de la lista inteligente para campañas inteligentes | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definición de la lista inteligente para campañas inteligentes | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

