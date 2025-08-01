---
unique-page-id: 2951877
description: 'Explicación del área de análisis de oportunidad de programa: documentos de Marketo, documentación del producto'
title: Explicación del área de análisis de oportunidad de programa
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 1%

---

# Explicación del área de análisis de oportunidad de programa {#understanding-the-program-opportunity-analysis-area}

## Información general {#overview}

El área Análisis de oportunidad de programa le permite analizar la eficacia de programas individuales o ver resultados resumidos por canal de programa.

**Las preguntas comerciales de ejemplo que puede responder con este área de análisis incluyen**:

¿Cuántas oportunidades se han asociado a un programa determinado y cuántas de ellas hemos ganado?

![](assets/one-1.png)

¿Cuántos ingresos ha ayudado a generar un programa o canal determinado?

![](assets/two-1.png)

¿Cuáles son mis ingresos de inversión para un programa o canal determinado?

![](assets/three-1.png)

¿En qué oportunidades influyó un programa determinado?

![](assets/four-1.png)

## Medidas de atribución de análisis de oportunidad de programa (puntos azules) {#program-opportunity-analysis-attribution-measures-blue-dots}

Las medidas disponibles para su uso en el análisis suelen ser números y se representan con puntos azules. Las dimensiones son atributos que proporcionan diferentes vistas de las medidas y que se representan con puntos amarillos.

Todas las medidas (puntos azules) están relacionadas con la atribución: el &quot;crédito&quot; por la adquisición de cliente potencial o por el éxito de ventas asociado a un cliente potencial.

![](assets/six.five.png) ![](assets/seven-1.png)

Existen tres tipos de medidas:

* Medidas relacionadas con la adquisición, que obtienen atribución de primer contacto (FT).
* Medidas relacionadas con el éxito, que reciben atribución multitáctil (MT).
* Varias medidas relacionadas con el programa, incluido el número promedio de toques de marketing antes de crear o cerrar Oportunidades.

## Adquisición y medidas relacionadas con el éxito {#acquisition-and-success-related-measures}

Las medidas relacionadas con la adquisición dan crédito al programa a través del cual se obtiene por primera vez la información de contacto de un posible cliente. Un posible cliente no tiene que lograr el éxito en un programa para que se conceda crédito de adquisición.

El valor de adquirir un posible cliente determinado cambia con el tiempo. Es cero hasta que el posible cliente realiza una compra. A continuación, puede aumentar con compras adicionales.

Las medidas relacionadas con el éxito dan crédito a todos los programas que contribuyen al progreso de un posible cliente hacia una compra.

Al igual que con la adquisición, el valor de la contribución a las ventas realizadas a un posible cliente cambia con el tiempo y es cero hasta que el posible cliente realiza alguna compra.

<table>
 <tbody>
  <tr>
   <th>Medida de atribución - Relacionada con la oportunidad (FT o MT)*</th>
   <th>Descripción</th>
  </tr>
  <tr>
   <td>Costo de oportunidad</td>
   <td>La parte del coste del programa que influyó en la oportunidad. El coste se puede dividir si hay varios posibles clientes implicados.</td>
  </tr>
  <tr>
   <td>Oportunidades creadas</td>
   <td>La parte de crédito que recibió el programa por influir en la creación de la oportunidad. Puede ser una fracción si hubo múltiples posibles clientes involucrados.</td>
  </tr>
  <tr>
   <td>Oportunidades ganadas</td>
   <td>La porción de crédito que recibió el programa por influir en la oportunidad ganada. Puede ser una fracción si hubo múltiples posibles clientes involucrados.</td>
  </tr>
  <tr>
   <td>Canalización creada</td>
   <td>La porción de crédito (en valor monetario) que recibió el programa por influir en la creación de la oportunidad. Puede ser una fracción si hubo múltiples posibles clientes involucrados.</td>
  </tr>
  <tr>
   <td>Canalización creada: aún abierta</td>
   <td>La porción de crédito (en valor monetario) que recibió el programa por influir en la creación de la oportunidad actualmente abierta. Puede ser una fracción si hubo múltiples posibles clientes involucrados.</td>
  </tr>
  <tr>
   <td>Ingresos esperados</td>
   <td>La porción de crédito (en valor monetario) que recibió el programa por influir en la creación de la oportunidad. Ingresos esperados es la probabilidad de oportunidad multiplicada por el valor de oportunidad. Puede ser una fracción si hubo múltiples posibles clientes involucrados.</td>
  </tr>
  <tr>
   <td>Ingresos a la inversión</td>
   <td>Se trata de la proporción de la parte del crédito (en valor monetario) que recibió el programa por influir en las oportunidades ganadas y el costo del programa.</td>
  </tr>
  <tr>
   <td>Ingresos obtenidos</td>
   <td>La porción de crédito (en valor monetario) que recibió el programa por influir en la oportunidad ganada. Puede ser una fracción si hubo múltiples posibles clientes involucrados.</td>
  </tr>
 </tbody>
</table>

_&#42;(FT) = Atribución de primer contacto, utilizada para medidas de adquisición de posibles clientes; (MT) = Atribución de varios contactos, utilizada para medidas de éxito de posibles clientes_

A continuación se muestra un escenario que describe cómo se calculan las unidades de oportunidad cuando hay dos programas que generaron posibles clientes, pero esos posibles clientes llevaron a una oportunidad desde la misma cuenta.

**Programa 1**

* Genera un posible cliente: posible cliente 1
* Posible cliente 1 es de Cuenta 1

**Programa 2**

* Genera otro posible cliente: posible cliente 2
* El posible cliente 2 también es de la cuenta 1

**Cuenta 1**

* Genera una oportunidad: oportunidad 1

Marketo otorga el crédito correctamente sin contar dos veces las oportunidades entre programas. Por lo tanto, en este caso, cada programa recibe 0,5 unidades de oportunidad. Es decir, cada Programa recibe la mitad del crédito por la oportunidad generada. Además, la mitad de los ingresos asociados con la oportunidad se asigna a cada programa.

## Medidas diversas relacionadas con los programas {#miscellaneous-program-related-measures}

Las demás medidas disponibles reflejan el rendimiento general del Programa.

<table>
 <tbody>
  <tr>
   <th>Medida de atribución: relacionada con el programa</th>
   <th>Descripción</th>
  </tr>
  <tr>
   <td>Cantidad de oportunidades asociadas al programa</td>
   <td><p>Número total de oportunidades que han dado algún tipo de crédito de atribución a un programa. Las oportunidades pueden verse influidas por uno o más posibles clientes y por uno o más programas.</p></td>
  </tr>
  <tr>
   <td>Cantidad promedio de éxitos por oportunidad cerrada</td>
   <td>Cantidad promedio de éxitos del programa antes de cerrar la oportunidad. <br></td>
  </tr>
  <tr>
   <td>Cantidad promedio de éxitos por oportunidad creada</td>
   <td>Cantidad promedio de programas ejecutados correctamente antes de crear la oportunidad.</td>
  </tr>
  <tr>
   <td>Nuevos nombres</td>
   <td>Número total de nuevos nombres, es decir, nuevos posibles clientes, adquiridos por el Programa.</td>
  </tr>
  <tr>
   <td>Costo del programa</td>
   <td>Coste total del programa.</td>
  </tr>
  <tr>
   <td>Éxito (total)</td>
   <td>Número total de miembros del programa que lograron el éxito.</td>
  </tr>
 </tbody>
</table>

## Dimensiones del análisis de oportunidad de programa (puntos amarillos) {#program-opportunity-analysis-dimensions-yellow-dots}

Mientras que las medidas (puntos azules) se calculan y requieren cierta reflexión y explicación, las dimensiones (puntos amarillos) son descriptivas. Estas son las dimensiones disponibles.

<table>
 <tbody>
  <tr>
   <th>Categoría</th>
   <th>Mostrar etiqueta</th>
  </tr>
  <tr>
   <td>Atributos de la oportunidad</td>
   <td>Oportunidad cerrada<br>Nombre de oportunidad*<br>Nombre de propietario de oportunidad<br>Fase de oportunidad<br>Tipo de oportunidad</td>
  </tr>
  <tr>
   <td>Periodo de oportunidad</td>
   <td>Oportunidad Cerrada Año/Trimestre/Mes<br>Oportunidad Creada Año/Trimestre/Mes</td>
  </tr>
  <tr>
   <td>Atributos del programa</td>
   <td>Canal de programa<br>Nombre de programa</td>
  </tr>
  <tr>
   <td>Intervalo de tiempo de costo de programa</td>
   <td>Año/Trimestre/Mes de coste</td>
  </tr>
 </tbody>
</table>

*&#42;Todas las oportunidades que dieron crédito de atribución de cualquier tipo a un programa. Las oportunidades pueden verse influidas por uno o más posibles clientes y por uno o más programas.*

>[!MORELIKETHIS]
>
>[Crear un informe de explorador de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
