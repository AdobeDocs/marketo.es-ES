---
unique-page-id: 2949413
description: Obtenga información sobre cómo agregar una restricción a un filtro de listas inteligentes. Refine los filtros con condiciones adicionales para obtener listas más precisas.
title: Añadir una restricción a un filtro de listas inteligentes
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/UqkPxJFs-78VaVMNgOa1p2sTuDo-FM74HXp3CAbruhA'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 10%
---
# Añadir una restricción a un filtro de listas inteligentes {#add-a-constraint-to-a-smart-list-filter}

Al crear una lista inteligente, algunos filtros tienen opciones avanzadas denominadas &quot;restricciones&quot;. Estas son condiciones adicionales que puede agregar a los filtros y déclencheur para ayudar a limitar la búsqueda aún más.

En este ejemplo, agregue algunas restricciones a un filtro **[Valor de datos cambiado](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** para encontrar personas que tuvieron un cambio de estado de MQL a SQL.

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Usar el filtro &quot;Valor de datos cambiado&quot; en una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. Seleccione la Smart List con un filtro al que agregará una restricción y haga clic en la ficha **[!UICONTROL Smart List]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. En **[!UICONTROL Agregar restricción]**, seleccione **[!UICONTROL Valor anterior]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. Escriba el **[!UICONTROL Valor anterior]**. En este ejemplo, utilizamos MQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. En **[!UICONTROL Agregar restricción]**, seleccione **[!UICONTROL Nuevo valor]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. Introduzca el nuevo valor. En este ejemplo, se utiliza SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. Haga clic en la ficha **[!UICONTROL Personas]** para ver todas las personas que han cambiado de estado de &quot;MQL&quot; a &quot;SQL&quot; en los últimos 30 días.
