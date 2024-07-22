---
unique-page-id: 2360421
description: Anular el comportamiento de Analytics en el nivel de programa - Documentos de Marketo - Documentación del producto
title: Anular el comportamiento de Analytics en el nivel de programa
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 1%

---

# Anular el comportamiento de Analytics en el nivel de programa {#override-analytics-behavior-at-the-program-level}

Puede establecer el comportamiento de [analytics en el nivel de administrador en los canales](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md), pero también puede anularlo en el nivel de programa. A continuación se muestra cómo:

1. Vaya al área de **Actividades de mercadotecnia**.

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. Busque y seleccione su programa.

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. En la ficha **Configuración**, arrastre Comportamiento de Analytics al lienzo.

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. Seleccione el Comportamiento de Analytics que desee.

   >[!NOTE]
   >
   >**Definición**
   >
   >* **Inclusivo**: esta opción garantizará que el programa esté disponible para la generación de informes en el explorador de ingresos y los analizadores, independientemente de si ha incluido o no un costo de período.
   >* **Operativo**: esta opción hace que el programa no se muestre en el explorador de ingresos ni en los analizadores.

   >[!NOTE]
   >
   >El comportamiento predeterminado (si no se aplica esta configuración) es que el programa se incluiría en Analytics **SOLAMENTE si hay al menos un costo de período**, incluso uno con cero dólares asignados.

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

¡Bien hecho! Ahora sabe cómo anular el comportamiento de análisis en el nivel de programa.

>[!NOTE]
>
>Los cambios entrarán en vigor el día siguiente y estarán disponibles o se retirarán del explorador de ingresos y de los analizadores.
