---
unique-page-id: 3571886
description: 'Uso del Analizador de rutas de éxito: Documentos de Marketo: Documentación del producto'
title: Uso del analizador de rutas de éxito
exl-id: f816b7ac-a158-46bd-9d00-09ef4cc8b381
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Uso del analizador de rutas de éxito {#using-the-success-path-analyzer}

Utilice un analizador de rutas de éxito para explorar los detalles específicos que reflejan tanto el flujo (cantidad) como la velocidad (velocidad, en términos de días) de las personas a través de las etapas del [Modelo de ciclo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

>[!PREREQUISITES]
>
>[Crear un analizador de rutas de éxito](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-success-path-analyzer.md)

1. Vaya a **Analytics** y seleccione **Analizador de rutas de éxito**.

   ![](assets/image2015-6-12-17-3a23-3a53.png)

   El gráfico de la derecha refleja los datos del botón seleccionado de la izquierda. De forma predeterminada, se trata de Balance.

1. Haga clic en **En flujo** para crear un gráfico de cuántas personas entraron al escenario durante el lapso de tiempo seleccionado.

   ![](assets/image2015-6-12-17-3a30-3a52.png)

   * Haga clic en Flujo para graficar cuántas personas salieron del escenario.
   * Haga clic en Conv % para graficar la tasa de conversión de esta a la siguiente etapa.
   * Haga clic en Promedio de tiempo para ver cuánto tiempo han pasado las personas en esta etapa antes de pasar al siguiente paso.

1. Haga clic en **Acciones de gráfico** > Comparar periodo para comparar los datos con un intervalo de tiempo diferente de igual longitud.

   ![](assets/image2015-6-12-17-3a39-3a15.png)

1. Seleccione el **De** fecha para el periodo de comparación.

   ![](assets/image2015-6-12-17-3a43-3a49.png)

   La variable **Hasta** se configura automáticamente para que coincida con la duración del período de tiempo original.

1. Haga clic en **Comparar**.

   ![](assets/image2015-6-12-17-3a44-3a8.png)

1. El gráfico se actualiza con datos superpuestos para el período de comparación, en verde.

   ![](assets/image2015-6-12-17-3a46-3a16.png)

1. Para cambiar la escala de tiempo del gráfico, haga clic en una de las **Gráfico por** botones: diariamente (predeterminado), semanalmente y mensualmente

   ![](assets/image2015-6-12-17-3a46-3a55.png)

1. Para etapas con SLAs (Acuerdos de Nivel de Servicio), haga clic en **Acciones de gráfico** > **Mostrar SLA vencido** para mostrar a todas las personas que alguna vez omitieron un objetivo de SLA dentro del lapso de tiempo especificado.

   ![](assets/image2015-6-12-17-3a49-3a23.png)

1. El gráfico se actualiza para reflejar cuántos SLAs se adeudaban en cada nodo, en naranja.

   ![](assets/image2015-6-12-17-3a50-3a16.png)

   La gente mostrada en naranja podría *o puede no* siga estando en la fase SLA.

1. Haga clic en **Acciones de gráfico** > **Mostrar SLA vencido** para mostrar todas las personas con objetivos SLA caducados que aún se encuentren en la fase SLA al final del período de tiempo especificado.

   ![](assets/image2015-6-12-17-3a51-3a39.png)

1. El gráfico se actualiza para reflejar cuántos SLAs se vencieron en cada nodo, en naranja.

   ![](assets/image2015-6-12-17-3a52-3a17.png)

1. Para leer los detalles específicos de un punto de datos en un nodo específico (fecha), pase el ratón sobre la burbuja.

   ![](assets/image2015-6-12-17-3a52-3a49.png)

1. Para imprimir el gráfico, haga clic en **Acciones de gráfico** > **Imprimir gráfico**.

   ![](assets/image2015-6-12-17-3a53-3a34.png)

El analizador está aquí para ayudarle a comprender el movimiento a través de su modelo. A medida que avance, esto será muy importante para diseñar estrategias de marketing.
