---
unique-page-id: 2949413
description: 'Agregar una restricción a un filtro de listas inteligentes: documentos de Marketo, documentación del producto'
title: Agregar una restricción a un filtro de listas inteligentes
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Agregar una restricción a un filtro de listas inteligentes {#add-a-constraint-to-a-smart-list-filter}

Al crear listas inteligentes, algunos filtros tienen opciones avanzadas denominadas &quot;restricciones&quot;. Estas son condiciones adicionales que puede agregar a los filtros y déclencheur para ayudar a limitar la búsqueda aún más.

En este ejemplo, vamos a añadir algunas restricciones a una **[Valor de datos cambiado](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** filtre para buscar personas que tuvieron un cambio de estado de MQL a SQL.

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Usar el filtro &quot;Valor de datos cambiado&quot; en una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>

1. Ir a **Actividades de marketing**.

   ![](assets/ma-1.png)

1. Seleccione la lista inteligente con un filtro al que desee agregar una restricción y haga clic en **Lista inteligente** pestaña.

   ![](assets/two-3.png)

1. En **Agregar restricción**, seleccione **Valor anterior**.

   ![](assets/three-3.png)

1. Introduzca el **Valor anterior**. En este ejemplo utilizamos MQL.

   ![](assets/four-2.png)

1. En **Agregar restricción**, seleccione **Nuevo valor**.

   ![](assets/five.png)

1. Introduzca el **Nuevo valor**. En este ejemplo utilizamos SQL.

   ![](assets/six.png)

1. ¡Bien hecho! Haga clic en **People** para ver todas las personas que tenían un **Estado** cambiar de **MQL** hasta **SQL** en los últimos 30 días.
