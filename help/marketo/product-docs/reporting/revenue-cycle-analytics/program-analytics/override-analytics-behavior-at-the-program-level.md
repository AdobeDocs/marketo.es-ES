---
unique-page-id: 2360421
description: Anular el comportamiento de Analytics en el nivel de programa - Documentos de Marketo - Documentación del producto
title: Anular el comportamiento de Analytics en el nivel de programa
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Anular el comportamiento de Analytics en el nivel de programa {#override-analytics-behavior-at-the-program-level}

Puede configurar la variable [comportamiento de analytics a nivel de administrador en canales](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md) pero también puede anularlo a nivel de programa. Así es como:

1. Vaya a la **Actividades de marketing** .

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. Busque y seleccione el programa.

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. En el **Configuración** , arrastre Comportamiento de Analytics al lienzo.

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. Seleccione el comportamiento de Analytics que desee.

   >[!NOTE]
   >
   >**Definición**
   >
   >* **Inclusivo** : esta opción garantiza que el programa esté disponible para informes en exploradores y analizadores de ingresos independientemente de si ha incluido o no un coste de período.
   >* **Operativo** : Esta opción hace que el programa no se muestre ni en el explorador de ingresos ni en los analizadores.


   >[!NOTE]
   >
   >El comportamiento predeterminado (si no se aplica esta configuración) es que el programa se incluiría en Analytics **SOLO si hay al menos un coste de período**, incluso uno con cero dólares asignados.

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

¡Bien hecho! Ahora sabe cómo anular el comportamiento de análisis en el nivel de programa.

>[!NOTE]
>
>Los cambios tendrán efecto al día siguiente y estarán disponibles o se extraerán de los exploradores y analizadores de ingresos.
