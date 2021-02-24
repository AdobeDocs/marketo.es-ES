---
unique-page-id: 2360423
description: Buscar todos los posibles clientes en un modelo de ciclo de ingresos - Documentos de marketing - Documentación del producto
title: Buscar todos los posibles clientes en un modelo de ciclo de ingresos
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---


# Buscar todos los posibles clientes en un modelo de ciclo de ingresos {#find-all-leads-in-a-revenue-cycle-model}

Mediante listas inteligentes, puede encontrar fácilmente todos los miembros del modelo de ciclo de ingresos.

>[!PREREQUISITES]
>
>[Crear una Lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Con la lista inteligente seleccionada, haga clic en la ficha **Lista inteligente**.

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. Busque el filtro **Miembro del modelo de ingresos** y arrástrelo al lienzo.

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. Seleccione un **Modelo**.

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   Esto les daría todos los leads en ese modelo, independientemente del escenario. Generalmente, querrá una etapa específica. Utilice el siguiente filtro en su lugar.

1. Busque el filtro **Fase de ingresos** y arrástrelo al lienzo.

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. Seleccione una **etapa**.

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. Vaya a la ficha **Posibles clientes** para vista de los resultados.

   ![](assets/2.png)

   >[!TIP]
   >
   >No necesitas ambos filtros, solo elige el que necesitas. Estamos demostrando que ambos son exhaustivos. ![(sonrisa)](assets/smile.svg)

   >[!CAUTION]
   >
   >Si la etapa de un posible cliente se cambia por una campaña externa durante la creación inicial del posible cliente, no se registra una actividad en la base de datos. Esto significa que el lista inteligente no incluirá el lead.
