---
unique-page-id: 7514009
description: 'Explicación del área de análisis de la fase de ingresos del programa: documentos de Marketo, documentación del producto'
title: Explicación del área de análisis de la fase Ingresos del programa
exl-id: 7310655f-a06e-4e02-a094-d942fff689c3
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 5%

---

# Explicación del área de análisis de la fase Ingresos del programa {#understanding-the-program-revenue-stage-analysis-area}

Esta área de análisis le permite analizar la eficacia de programas individuales o ver resultados resumidos por canal. Proporciona información sobre cuántos de los nuevos nombres generados han alcanzado fases de ruta de éxito específicas dentro del modelo de ciclo de ingresos.

**Las preguntas comerciales de ejemplo que puede responder con este área de análisis incluyen**:

¿Cuántos nombres nuevos de un programa determinado han alcanzado alguna vez una fase específica en mi modelo?

![](assets/one-3.png)

¿Cuántos nombres nuevos de un programa determinado se encuentran actualmente en una fase específica de mi modelo?

![](assets/two-3.png)

¿Cuántos días están tardando los posibles clientes en llegar a su fase actual?

![](assets/three-3.png)

**Dimensiones y medidas del análisis de fase de ingresos del programa**

Las dimensiones y las medidas se clasifican por funcionalidad y se representan con puntos amarillos o azules en el sistema: amarillo para las dimensiones y azul para las medidas. Utilice dimensiones y medidas de análisis de la fase de ingresos del programa para responder preguntas específicas en el informe.

Para ver las dimensiones o medidas disponibles dentro de una categoría, haga clic en la flecha derecha junto al nombre de una categoría para expandir la lista de categorías. Haga clic en la flecha hacia abajo para contraer la lista de categorías.

>[!TIP]
>
>Para obtener más información sobre una dimensión o medida en particular mientras está en el informe, pase el ratón sobre ella.

**Atributos de modelo**

<table>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong>Dimensión</strong></td>
   <td colspan="1" rowspan="1"><p><strong>Descripción</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>El modelo está activo</p></td>
   <td colspan="1" rowspan="1"><p>Describe si el modelo está aprobado y activo actualmente</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Está activo el escenario</p></td>
   <td colspan="1" rowspan="1"><p>Describe si la fase está activa</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>En ruta de éxito</p></td>
   <td colspan="1" rowspan="1"><p>Describe si la fase está en la ruta de éxito o no</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Modelo</p></td>
   <td colspan="1" rowspan="1"><p>Nombre de modelo</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Fase</p></td>
   <td colspan="1" rowspan="1"><p>Las fases que existen en el modelo del ciclo de ingresos. Se utiliza como fase Desde al analizar medidas entre dos fases</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Tipo de escenario</p></td>
   <td colspan="1" rowspan="1"><p>Describe el tipo; inventario, SLA o puerta en cada fase</p></td>
  </tr>
 </tbody>
</table>

**Atributos del programa**

<table>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Dimensión</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>Descripción</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Canal del programa</p></td>
   <td colspan="1" rowspan="1"><p>Canal del programa</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Nombre del programa</p></td>
   <td colspan="1" rowspan="1"><p>Nombre del programa</p></td>
  </tr>
 </tbody>
</table>

**Período de tiempo de costo del programa**

<table>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Dimensión</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>Descripción</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Año de coste</p></td>
   <td colspan="1" rowspan="1"><p>Plazo de coste del programa</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Trimestre de coste</p></td>
   <td colspan="1" rowspan="1"><p>Plazo de coste del programa</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Mes de coste</p></td>
   <td colspan="1" rowspan="1"><p>Plazo de coste del programa</p></td>
  </tr>
 </tbody>
</table>

**Pertenencia a la fase**

<table>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Medida</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>Descripción</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>El modelo está activo</p></td>
   <td colspan="1" rowspan="1"><p>Describe si el modelo está aprobado y activo actualmente</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Está activo el escenario</p></td>
   <td colspan="1" rowspan="1"><p>Describe si la fase está activa</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>En ruta de éxito</p></td>
   <td colspan="1" rowspan="1"><p>Describe si la fase está en la ruta de éxito o no</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Costo por nombre nuevo</p></td>
   <td colspan="1" rowspan="1"><p>El coste medio de un nuevo nombre que alguna vez llegó a la fase</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Nuevos nombres (actuales)</p></td>
   <td colspan="1" rowspan="1"><p>Número total de posibles clientes que se encuentran actualmente en la fase y que fueron adquiridos por el programa</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p>Nuevos nombres (siempre)</p></td>
   <td colspan="1" rowspan="1"><p>Describe el tipo; inventario, SLA o puerta en cada fase</p></td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Crear un informe de explorador de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
