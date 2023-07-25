---
unique-page-id: 2360389
description: Disponibilidad de un programa sin coste de período en el Explorador de ingresos y Analizadores - Documentos de Marketo - Documentación del producto
title: Disponibilidad de un programa sin coste de período en el Explorador de ingresos y en los analizadores
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Disponibilidad de un programa sin coste de período en el Explorador de ingresos y en los analizadores {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Costos de período del programa le permite definir &quot;Cuánto dinero&quot; y &quot;Cuándo&quot; para un programa. Esto aparece en el Explorador de ciclos de ingresos y [analizadores](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Permisos de administración necesarios**

Es posible que algunos programas deban incluirse incluso si no tienen un coste de periodo. Aunque puede escribir 0 para el coste del período, hemos facilitado la inclusión de estos programas.

>[!NOTE]
>
>El analizador de programas agrupa el éxito del programa por coste de periodo. Si no hay ningún costo de período disponible, no se mostrará Éxito del programa, independientemente del comportamiento de análisis del programa. Si se configura el comportamiento del análisis, los datos se mostrarán para las métricas de oportunidad (oportunidades de canalización, ingresos obtenidos, etc.).

1. En la sección Administración, haga clic en **Etiquetas**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Expanda los canales y haga doble clic en el canal que desee.

   >[!NOTE]
   >
   >Todos los programas que utilicen este canal, independientemente del coste del periodo, estarán disponibles para el explorador de ingresos y los analizadores. Este cambio entra en vigor al día siguiente.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Cambie el comportamiento de Analytics a Inclusivo y haga clic en **Guardar**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>¿Se ha fijado en la opción Operativo? Esto hace lo contrario. Excluye estos programas independientemente del coste del periodo.

¡Buen trabajo! Ahora, cualquier programa que utilice el canal modificado se incluirá en el explorador de ingresos y en los analizadores sin necesidad de un coste de periodo.

>[!MORELIKETHIS]
>
>[Anular el comportamiento de Analytics en el nivel de programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
