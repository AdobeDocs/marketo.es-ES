---
unique-page-id: 2949413
description: Agregar una restricción a un filtro de lista inteligente - Documentos de Marketo - Documentación del producto
title: Agregar una restricción a un filtro de lista inteligente
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Agregar una restricción a un filtro de lista inteligente {#add-a-constraint-to-a-smart-list-filter}

Al crear listas inteligentes, algunos filtros tienen opciones avanzadas llamadas &quot;restricciones&quot;. Estas son condiciones adicionales que puede agregar a los filtros y déclencheur para ayudar a limitar aún más la búsqueda.

En este ejemplo, vamos a agregar algunas restricciones a un **[Valor de datos cambiado](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** para buscar personas que hayan cambiado de estado de MQL a SQL.

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Utilizar el filtro &quot;Data Value Changed&quot; en una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>


1. Vaya a **Actividades de marketing**.

   ![](assets/ma-1.png)

1. Seleccione la lista inteligente con un filtro al que agregará una restricción y haga clic en el botón **Lista inteligente** pestaña .

   ![](assets/two-3.png)

1. En **Agregar restricción**, seleccione **Valor anterior**.

   ![](assets/three-3.png)

1. Introduzca la variable **Valor anterior**. En este ejemplo utilizamos MQL.

   ![](assets/four-2.png)

1. En **Agregar restricción**, seleccione **Nuevo valor**.

   ![](assets/five.png)

1. Introduzca la variable **Nuevo valor**. En este ejemplo utilizamos SQL.

   ![](assets/six.png)

1. ¡Bien hecho! Haga clic en el **People** para ver todas las personas que tenían una **Estado** cambiar de **MQL** a **SQL** en los últimos 30 días.
