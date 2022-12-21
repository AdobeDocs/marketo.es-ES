---
unique-page-id: 2360389
description: Hacer que un programa sin costo de período esté disponible en el Explorador de ingresos y analizadores - Documentos de Marketo - Documentación del producto
title: Hacer que un programa sin costo de período esté disponible en el Explorador de ingresos y analizadores
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Hacer que un programa sin costo de período esté disponible en el Explorador de ingresos y analizadores {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Los costos de período de programa le permiten definir &quot;Cuánto dinero&quot; y &quot;Cuándo&quot; para un programa. Esto se muestra en el Explorador de ciclo de ingresos y [analizadores](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Se requieren permisos de administrador**

Es posible que algunos programas deban incluirse aunque no tengan un costo de período. Aunque puede introducir 0 para el coste del periodo, hemos facilitado la inclusión de estos programas.

>[!NOTE]
>
>El Analizador de programas agrupa el éxito del programa por coste de período. Si no hay ningún coste de período disponible, el éxito del programa no se mostrará, independientemente del comportamiento analítico del programa. Si se configura el comportamiento de análisis, se mostrarán datos para métricas de oportunidad (oportunidades de canalización, ingresos obtenidos, etc.).

1. En la sección Administración , haga clic en **Etiquetas**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Expanda los canales y haga doble clic en el canal que desee.

   >[!NOTE]
   >
   >Todos los programas que utilicen este canal, independientemente del coste de período, estarán disponibles para los analizadores y exploradores de ingresos. Este cambio tendrá efecto al día siguiente.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Cambie el comportamiento de Analytics a Inclusivo y haga clic en **Guardar**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>¿Ha notado la opción Operativo? Esto hace lo contrario. Excluye estos programas independientemente del costo del período.

¡Buen trabajo! Ahora, cualquier programa que utilice el canal modificado se incluirá en el explorador de ingresos y en los analizadores sin necesidad de un coste de período.

>[!MORELIKETHIS]
>
>[Anular el comportamiento de Analytics en el nivel de programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
