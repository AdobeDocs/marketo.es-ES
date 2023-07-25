---
unique-page-id: 1146940
description: Definición de listas inteligentes para campañas inteligentes | Lote - Documentos de Marketo - Documentación del producto
title: Definición de listas inteligentes para campañas inteligentes | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Definición de listas inteligentes para campañas inteligentes | Lote {#define-smart-list-for-smart-campaign-batch}

Las listas inteligentes son el mecanismo que utiliza Marketo para definir &quot;quién&quot; (qué personas) incluir, ya sea un informe, una lista o una campaña inteligente. A continuación se indica cómo definir una lista inteligente para una campaña por lotes.

1. Elija una campaña inteligente y haga clic en **Lista inteligente**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Escriba para buscar un filtro y arrástrelo y suéltelo en el lienzo. Repita el proceso para varios filtros.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Se ejecuta una campaña inteligente con solo filtros en **Lote** modo. Encuentra personas en la base de datos que cumplen los requisitos en función de los filtros y las ejecuta todas a través del flujo a la vez.

   >[!NOTE]
   >
   >Puede hacer que una campaña inteligente se ejecute en una persona a la vez en función de los eventos en directo añadiendo déclencheur, lo que coloca la campaña inteligente en **Déclencheur** modo.

1. Haga clic en la lista desplegable y seleccione un operador de filtro para el filtro que haya elegido.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Las líneas rojas onduladas indican errores o falta información. Si no se corrige, la campaña no será válida y no se ejecutará.

1. Introduzca el valor de filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >De forma predeterminada, se cualifican las personas que cumplen TODAS las reglas de listas inteligentes. Puede modificarla para adaptarla a sus necesidades de campaña. Desproteger  [Reglas de listas inteligentes para lógica compleja](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) para obtener más información.

   Para recibir déclencheur en eventos en directo de una persona a la vez, aprenda a [Definición de listas inteligentes para campañas inteligentes | DÉCLENCHEUR](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definición de listas inteligentes para campañas inteligentes | DÉCLENCHEUR](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
