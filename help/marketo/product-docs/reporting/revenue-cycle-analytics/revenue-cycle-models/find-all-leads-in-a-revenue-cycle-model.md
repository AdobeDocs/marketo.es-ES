---
unique-page-id: 2360423
description: Obtenga información sobre cómo encontrar todos los posibles clientes en un modelo del ciclo de ingresos en Marketo Engage mediante Buscar todos los posibles clientes en un ciclo de ingresos. Utilice esta guía para completar el siguiente paso.
title: Buscar todos los posibles clientes en un modelo del ciclo de ingresos
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
feature: Reporting, Revenue Cycle Analytics
source-git-commit: f1b147b6883e5e150603304ba92b902125fea2b0
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 8%

---

# Buscar todos los posibles clientes en un modelo del ciclo de ingresos {#find-all-leads-in-a-revenue-cycle-model}

Mediante listas inteligentes, puede encontrar fácilmente todos los miembros del modelo de ciclo de ingresos.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Con la lista inteligente seleccionada, haga clic en la ficha **[!UICONTROL Lista inteligente]**.

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. Busque el filtro **[!UICONTROL Miembro del modelo de ingresos]** y arrástrelo al lienzo.

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. Seleccionar un **[!UICONTROL modelo]**.

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   Esto le daría todos los posibles clientes de ese modelo, independientemente del escenario. Por lo general, usted querrá una etapa específica. Utilice el siguiente filtro en su lugar.

1. Busque el filtro **[!UICONTROL Ingreso Stage]** y arrástrelo al lienzo.

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. Seleccione un **[!UICONTROL escenario]**.

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. Vaya a la pestaña **[!UICONTROL Posibles clientes]** para ver los resultados.

   ![](assets/2.png)

   >[!TIP]
   >
   >No necesita ambos filtros, solo elija el que necesita. Solo les estamos mostrando a ambos que sean minuciosos.

   >[!CAUTION]
   >
   >Si una campaña externa cambia la fase de un posible cliente durante la creación inicial de este, la actividad no se registra en la base de datos. Esto significa que el posible cliente no se incluirá en el filtro de lista inteligente.
