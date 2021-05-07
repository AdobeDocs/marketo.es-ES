---
unique-page-id: 2360423
description: 'Buscar todos los posibles clientes en un modelo de ciclo de ingresos: Documentos de Marketo: Documentación del producto'
title: Buscar todos los posibles clientes en un modelo de ciclo de ingresos
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
translation-type: tm+mt
source-git-commit: c1b2a5966da3bda18a2ccaab9b348296ba1d7bfd
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Buscar todos los posibles clientes en un modelo de ciclo de ingresos {#find-all-leads-in-a-revenue-cycle-model}

Mediante listas inteligentes, puede encontrar fácilmente todos los miembros del modelo de ciclo de ingresos.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Con la lista inteligente seleccionada, haga clic en la pestaña **Smart List**.

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. Busque el filtro **Member of Revenue Model** y arrástrelo al lienzo.

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. Seleccione un **Model**.

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   Esto les daría todos los posibles clientes en ese modelo, independientemente del escenario. Normalmente, desea una fase específica. Utilice el siguiente filtro en su lugar.

1. Busque el filtro **Revenue Stage** y arrástrelo al lienzo.

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. Seleccione un **Stage**.

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. Vaya a la pestaña **Leads** para ver los resultados.

   ![](assets/2.png)

   >[!TIP]
   >
   >No necesita ambos filtros, simplemente elija el que necesita. Sólo les estamos mostrando que son minuciosos.

   >[!CAUTION]
   >
   >Si la fase de un posible cliente cambia mediante una campaña externa durante la creación inicial del posible cliente, la actividad no se registra en la base de datos. Esto significa que el filtro de lista inteligente no incluirá el posible cliente.
