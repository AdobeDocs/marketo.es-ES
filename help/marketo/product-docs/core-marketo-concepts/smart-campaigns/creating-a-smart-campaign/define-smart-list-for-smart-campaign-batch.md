---
unique-page-id: 1146940
description: 'Definición de listas inteligentes para campañas inteligentes | Lote: Documentos de Marketo: documentación del producto'
title: Definición de listas inteligentes para campañas inteligentes | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: c3aa1a29b084cb1c1add9d22cdbfc23bdcf7512b
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Definición de listas inteligentes para campañas inteligentes | Lote {#define-smart-list-for-smart-campaign-batch}

Las listas inteligentes son el mecanismo a través del Marketo Engage para definir &quot;quién&quot; (qué personas) incluir, ya sea un informe, una lista o una campaña inteligente. A continuación se indica cómo definir una lista inteligente para una campaña por lotes.

>[!CAUTION]
>
>Realizar ediciones de listas inteligentes o pasos de flujo en una campaña activa puede dañar potencialmente su funcionalidad. Si decide hacerlo, proceda con precaución.

1. Elija una campaña inteligente y luego haga clic en **[!UICONTROL Lista inteligente]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Escriba para buscar un filtro y arrástrelo y suéltelo en el lienzo. Repita el proceso para varios filtros.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Se ejecuta una campaña inteligente que solo tiene filtros en modo _Batch_. Encuentra personas en la base de datos que cumplen los requisitos en función de los filtros y las ejecuta todas a través del flujo a la vez.

   >[!NOTE]
   >
   >Puede hacer que una campaña inteligente se ejecute en una persona a la vez en función de eventos en directo agregando déclencheur, lo que pone la campaña inteligente en modo _Déclencheur_.

1. Haga clic en la lista desplegable y seleccione un operador de filtro para el filtro que haya elegido.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Las líneas rojas onduladas indican errores o falta información. Si no se corrige, la campaña no será válida y no se ejecutará.

1. Introduzca el valor de filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >De forma predeterminada, se cualifican las personas que cumplen TODAS las reglas de listas inteligentes. Puede modificarla para adaptarla a sus necesidades de campaña. Consulte [Reglas de listas inteligentes para lógica compleja](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} para obtener más información.

   Para obtener déclencheur en eventos en vivo de una persona a la vez, aprenda a [Definir listas inteligentes para campañas inteligentes | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Definir lista inteligente para campaña inteligente | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Agregar un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
