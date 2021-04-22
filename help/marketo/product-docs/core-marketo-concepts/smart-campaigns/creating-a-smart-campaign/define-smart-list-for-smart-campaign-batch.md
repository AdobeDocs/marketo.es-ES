---
unique-page-id: 1146940
description: Definición de la lista inteligente para campañas inteligentes | Lote - Documentos de Marketo - Documentación del producto
title: Definición de la lista inteligente para campañas inteligentes | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Definición de la lista inteligente para campañas inteligentes | Lote {#define-smart-list-for-smart-campaign-batch}

Las listas inteligentes son el mecanismo de Marketo para definir &quot;quién&quot; (qué personas) incluir, ya sea un informe, una lista o una campaña inteligente. A continuación se muestra cómo definir una lista inteligente para una campaña por lotes.

1. Elija una campaña inteligente y haga clic en **Smart List**.

   ![](assets/campaignchoose-hand.png)

1. Escriba para buscar un filtro y luego arrástrelo y suéltelo en el lienzo. Repita el proceso para varios filtros.

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >Una campaña inteligente con solo filtros se ejecuta en modo **Batch**. Encuentra personas en la base de datos que califican según los filtros y los ejecuta a través del flujo a la vez.

   >[!NOTE]
   >
   >Puede hacer que una campaña inteligente se ejecute en una persona a la vez según los eventos en directo añadiendo déclencheur, lo que coloca la campaña inteligente en modo **Déclencheur**.

1. Haga clic en la lista desplegable y elija un operador de filtro para el filtro que ha elegido.

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >Las líneas rojas indican errores o falta información. Si no se corrige, la campaña no será válida y no se ejecutará.

1. Introduzca el valor del filtro.

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >De forma predeterminada, las personas que satisfacen TODAS las reglas de listas inteligentes están cualificadas. Esto se puede modificar para adaptarlo a sus necesidades de campaña. Consulte [Reglas de lista inteligente para lógica compleja](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) para obtener más información.

   Para realizar déclencheur en eventos en directo de una persona a la vez, aprenda a [Definir lista inteligente para campañas inteligentes | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definición de la lista inteligente para campañas inteligentes | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

