---
unique-page-id: 2949413
description: 'Agregar una restricción a un filtro de listas inteligentes: documentos de Marketo, documentación del producto'
title: Agregar una restricción a un filtro de listas inteligentes
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Agregar una restricción a un filtro de listas inteligentes {#add-a-constraint-to-a-smart-list-filter}

Al crear una lista inteligente, algunos filtros tienen opciones avanzadas denominadas &quot;restricciones&quot;. Estas son condiciones adicionales que puede agregar a los filtros y déclencheur para ayudar a limitar la búsqueda aún más.

En este ejemplo, vamos a agregar algunas restricciones a un filtro de **[Valor de datos cambiado](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** para encontrar personas que tuvieron un cambio de estado de MQL a SQL.

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

1. ¡Bien hecho! Haga clic en la ficha **[!UICONTROL Personas]** para ver todas las personas que han cambiado de estado de &quot;MQL&quot; a &quot;SQL&quot; en los últimos 30 días.
