---
unique-page-id: 2951877
description: 'Información sobre el área de análisis de oportunidades de programa: documentos de Marketo: documentación del producto'
title: Explicación del área de análisis de oportunidades del programa
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Explicación del área de análisis de oportunidades del programa {#understanding-the-program-opportunity-analysis-area}

## Resumen {#overview}

El área de Análisis de oportunidades del programa le permite analizar la eficacia de los programas individuales o ver los resultados resumidos por Canal del programa.

**Algunas preguntas comerciales de ejemplo que puede responder con esta área de análisis incluyen**:

¿Cuántas oportunidades se asociaron a un determinado Programa y cuántas de ellas hemos ganado?

![](assets/one-1.png)

¿Cuántos ingresos ha ayudado a generar un determinado Programa o Canal?

![](assets/two-1.png)

¿Cuáles son mis ingresos por inversión para un determinado programa o canal?

![](assets/three-1.png)

¿Qué oportunidades influyó un determinado Programa?

![](assets/four-1.png)

## Medidas de atribución del análisis de oportunidad del programa (puntos azules) {#program-opportunity-analysis-attribution-measures-blue-dots}

Las medidas disponibles para su uso en análisis son generalmente números y se representan con puntos azules. Los Dimension son atributos que proporcionan diferentes vistas de las medidas y que se representan mediante puntos amarillos.

Todas las medidas (puntos azules) están relacionadas con la atribución: el &quot;crédito&quot; para la adquisición de posibles clientes o para el éxito de ventas asociado a un posible cliente.

![](assets/six.five.png) ![](assets/seven-1.png)

Existen tres tipos de medidas:

* Medidas relacionadas con la adquisición, que obtienen atribución de primer contacto (FT).
* Medidas relacionadas con el éxito, que reciben atribución multitáctil (MT).
* Otras medidas relacionadas con el Programa, incluido el número promedio de toques de marketing antes de crear o cerrar Oportunidades.

## Adquisición y medidas relacionadas con el éxito {#acquisition-and-success-related-measures}

Las medidas relacionadas con la adquisición dan crédito al programa mediante el cual se obtiene por primera vez la información de contacto de un posible cliente. Un posible cliente no tiene que lograr el éxito en un programa para la concesión de créditos de adquisición.

El valor de adquirir un posible cliente determinado cambia con el tiempo. Es cero hasta que el cliente potencial realiza una compra. Luego puede aumentar con compras adicionales.

Las medidas relacionadas con el éxito dan crédito a todos los programas que contribuyen al progreso de un posible cliente hacia una compra.

Al igual que con la adquisición, el valor de contribuir a las ventas realizadas a un posible cliente cambia con el tiempo y es cero hasta que el cliente potencial realiza alguna compra.

<table> 
 <tbody> 
  <tr> 
   <th>Medida de atribución - Relacionada con oportunidades (FT o MT)*</th> 
   <th>Descripción</th> 
  </tr> 
  <tr> 
   <td>Costo de oportunidad</td> 
   <td>La parte del costo del programa que influyó en la oportunidad. El coste puede dividirse si hay varios posibles clientes implicados.</td> 
  </tr> 
  <tr> 
   <td>Oportunidades creadas</td> 
   <td>La parte del crédito que recibió el programa por influir en la creación de la oportunidad. Puede ser una fracción si hay múltiples pistas involucradas.</td> 
  </tr> 
  <tr> 
   <td>Oportunidades ganadas</td> 
   <td>La parte del crédito que recibió el programa por influir en la oportunidad que se le ofreció. Puede ser una fracción si hay múltiples pistas involucradas.</td> 
  </tr> 
  <tr> 
   <td>Canalización creada</td> 
   <td>La porción de crédito (en valor monetario) que el programa recibió por influir en la creación de la oportunidad. Puede ser una fracción si hay múltiples pistas involucradas.</td> 
  </tr> 
  <tr> 
   <td>Canalización creada: aún abierta</td> 
   <td>La porción de crédito (en valor monetario) que el programa recibió para influir en la creación de la oportunidad actualmente abierta. Puede ser una fracción si hay múltiples pistas involucradas.</td> 
  </tr> 
  <tr> 
   <td>Ingresos esperados</td> 
   <td>La porción de crédito (en valor monetario) que el programa recibió por influir en la creación de la oportunidad. Ingresos esperados es la probabilidad de oportunidad multiplicada por el valor de oportunidad. Puede ser una fracción si hay múltiples pistas involucradas.</td> 
  </tr> 
  <tr> 
   <td>Ingresos Por Inversión</td> 
   <td>Esta es la proporción de la parte del crédito (en valor monetario) que el programa recibió para influir en las oportunidades ganadas y el costo del programa.</td> 
  </tr> 
  <tr> 
   <td>Ganancias</td> 
   <td>La porción de crédito (en valor monetario) que el programa recibió por influir en las oportunidades ganadas. Puede ser una fracción si hay múltiples pistas involucradas.</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) = Atribución de primer toque, utilizada para medidas de adquisición de plomo; (MT) = Atribución multitáctil, utilizada para medir el éxito de los clientes_

A continuación se muestra un escenario que describe cómo se calculan las unidades de oportunidad cuando hay dos programas que generan posibles clientes, pero que generan una oportunidad desde la misma cuenta.

**Programa 1**

* Genera un posible cliente: Posible cliente 1
* El posible cliente 1 es de la cuenta 1

**Programa 2**

* Genera otro posible cliente: Posible cliente 2
* El posible cliente 2 también es de la cuenta 1

**Cuenta 1**

* Genera una oportunidad: Oportunidad 1

Marketo otorga crédito de forma adecuada sin tener que contar las oportunidades de forma doble entre programas. Por lo tanto, en este caso, cada Programa recibe 0,5 unidades de oportunidad. Es decir, cada Programa recibe la mitad del crédito por la oportunidad generada. Además, la mitad de los ingresos asociados con la oportunidad se asignan a cada programa.

## Medidas diversas relacionadas con los programas {#miscellaneous-program-related-measures}

Las demás medidas disponibles reflejan el desempeño general del Programa.

<table> 
 <tbody> 
  <tr> 
   <th>Medida de atribución - Relacionada con el programa</th> 
   <th>Descripción</th> 
  </tr> 
  <tr> 
   <td>N.º de oportunidades asociadas al programa</td> 
   <td><p>Número total de oportunidades que han concedido algún tipo de crédito de atribución a un programa. Las oportunidades pueden verse influidas por uno o más posibles clientes y por uno o más programas.</p></td> 
  </tr> 
  <tr> 
   <td>Promedio de éxitos por oportunidad cerrada</td> 
   <td>El número promedio de éxitos del Programa antes de que se cerrara la oportunidad. <br></td> 
  </tr> 
  <tr> 
   <td>Promedio de éxitos por oportunidad creada</td> 
   <td>Número promedio de programas exitosos antes de crear la oportunidad.</td> 
  </tr> 
  <tr> 
   <td>Nuevos nombres</td> 
   <td>Número total de nuevos nombres, es decir, nuevos posibles clientes, adquiridos por el Programa.</td> 
  </tr> 
  <tr> 
   <td>Coste del programa</td> 
   <td>Coste total del Programa.</td> 
  </tr> 
  <tr> 
   <td>Éxito (total)</td> 
   <td>Número total de miembros del Programa que lograron el éxito.</td> 
  </tr> 
 </tbody> 
</table>

## Dimension del análisis de oportunidades del programa (puntos amarillos) {#program-opportunity-analysis-dimensions-yellow-dots}

Mientras que las medidas (puntos azules) se calculan y requieren cierta reflexión y explicación para su uso, las dimensiones (puntos amarillos) son descriptivas. Estas son las dimensiones disponibles.

<table> 
 <tbody> 
  <tr> 
   <th>Categoría</th> 
   <th>Mostrar etiqueta</th> 
  </tr> 
  <tr> 
   <td>Atributos de oportunidad</td> 
   <td>Oportunidad cerrada<br>Nombre de oportunidad*<br>Nombre del propietario de la oportunidad<br>Fase de oportunidad<br>Tipo de oportunidad</td> 
  </tr> 
  <tr> 
   <td>Intervalo de tiempo de oportunidad</td> 
   <td>Oportunidad Año/Trimestre/Mes cerrado<br>Oportunidad creada año/trimestre/mes</td> 
  </tr> 
  <tr> 
   <td>Atributos del programa</td> 
   <td>Canal de programa<br>Nombre del programa</td> 
  </tr> 
  <tr> 
   <td>Intervalo de tiempo del costo del programa</td> 
   <td>Año/trimestre/mes de costo</td> 
  </tr> 
 </tbody> 
</table>

*&#42;Todas las oportunidades que le dieron cualquier tipo de crédito de atribución a un Programa. Las oportunidades pueden verse influidas por uno o más posibles clientes y por uno o más programas.*

>[!MORELIKETHIS]
>
>[Creación de un informe del Explorador de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
