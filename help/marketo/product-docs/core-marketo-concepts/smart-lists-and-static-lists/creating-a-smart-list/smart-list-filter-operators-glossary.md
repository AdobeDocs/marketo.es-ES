---
unique-page-id: 557312
description: Glosario de operadores de filtros de listas inteligentes - Documentos de Marketo - Documentación del producto
title: Glosario de operadores de filtros de listas inteligentes
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
source-git-commit: 5ffb1a1931ccbc945ba535f72898a1b73154e47a
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 12%

---

# Glosario de operadores de filtros de listas inteligentes {#smart-list-filter-operators-glossary}

Un operador es una parte de la lista inteligente que le ayuda a obtener información específica. Permite describir el filtro o déclencheur en un lenguaje sencillo. Los operadores disponibles son diferentes para cada tipo de campo.

Este glosario describe cada conjunto de operadores.

## Campos de fecha {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Al elegir un operador, el lado derecho cambia de forma dinámica.

| Operador | Lado derecho | Descripción |
|---|---|---|
| es | Fecha única | Coincidencia de fecha exacta |
| no es/no está | Fecha única | Cualquier fecha excepto la especificada |
| entre | Dos campos de fecha | Cualquier fecha, incluidas y entre dos fechas especificadas |
| en el pasado | Entrada de lenguaje natural&#42; | Consulte el diagrama siguiente |
| en el pasado, antes de | Entrada de lenguaje natural&#42; | Consulte el diagrama siguiente |
| en el futuro | Entrada de lenguaje natural&#42; | Consulte el diagrama siguiente |
| en el futuro, después de | Entrada de lenguaje natural&#42; | Consulte el diagrama siguiente |
| en el lapso de tiempo | Ajustes preestablecidos (último trimestre, ayer, etc.) | Definido en la lista de selección |
| después | Fecha única | Todos los registros posteriores a la fecha especificada |
| antes | Fecha única | Todos los registros anteriores al especificado |
| el o después de | Fecha única | Igual que &quot;después&quot;, pero inclusivo |
| el o antes del | Fecha única | Igual que &quot;antes&quot; pero inclusivo |
| está vacío | Ninguno | Todos los registros sin fecha |
| no está vacío | Ninguno | Todos los registros con cualquier fecha |

&#42; La entrada de lenguaje natural es genial. Estos son algunos de los patrones que puede introducir:

* 1 hora
* 82 días
* 3 semanas
* 14 meses
* 1 año

Solo escribe el número y la unidad juntos y va a funcionar!

>[!NOTE]
>
>&quot;En el pasado&quot; **hace** incluya el día (hasta el momento, no después) en que crea la lista inteligente.

>[!CAUTION]
>
>Cuando crea una lista inteligente utilizando un filtro de campo de fecha (por ejemplo, Fecha de nacimiento, Fecha de creación de SFDC) y utiliza las restricciones **antes**, **el o antes**, o **en el pasado antes**, la lista inteligente también incluirá a las personas que no tengan ningún valor en dicho campo de fecha.

Utilice el diagrama siguiente para comprender la diferencia entre los operadores de fecha.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Ejemplo**
>
>Los campos de fecha pueden resultar complicados cuando se trabaja con eventos pasados y futuros. Aquí hay un par de ejemplos.
>
>**Antes de**
>
>Para la nueva promoción, utilice este operador para enviar correos electrónicos solo a las personas que no se hayan suscrito o renovado el servicio en el plazo de un año o que nunca se hayan suscrito.
>
>**En el futuro después de**
>
>Supongamos que desea ver los clientes que se van a renovar en 90 días. Se utilizan dos filtros independientes. Primero use &quot;En el futuro después de 90 días&quot; y segundo, &quot;En el futuro en 91 días&quot;. Eso capturaría a quien tenga una cita dentro de 90 días.

## Campos de cadena {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operador | Descripción |
|---|---|
| es | Coincidencia exacta (sin distinción de mayúsculas y minúsculas) |
| no es/no está | Cualquier cosa excepto coincidencia exacta |
| comienza con | Coincidencia de las primeras letras de la cadena |
| no comienza con | Las primeras letras de la cadena NO coinciden |
| contiene | Cualquier letra de la cadena coincide (por ejemplo: california, queue, etc.) |
| no contiene | No hay letras juntas en la cadena que coincidan. (al revés de &quot;contiene&quot;) |
| está vacío | Registros sin valor (NULL) |
| no está vacío | Registros con valor ANY |

>[!TIP]
>
>Utilice operadores positivos sobre negativos. Los filtros &quot;No es&quot; tienen que buscar todo el conjunto de datos en su instancia, lo que puede consumir mucho tiempo. Los filtros positivos &quot;es&quot; pueden aprovechar algoritmos de búsqueda más eficaces.

## Campos enteros {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Operador</th> 
   <th colspan="1" rowspan="1">Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">es</td> 
   <td colspan="1" rowspan="1">La coincidencia de número exacto ( = 0 devolverá ambos posibles clientes con 0 <em>y</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no es/no está</td> 
   <td colspan="1" rowspan="1">Cualquier cosa EXCEPTO el número exacto coincide</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">entre</td> 
   <td colspan="1" rowspan="1">Defina dos valores para encontrar a todos los que estén en el medio (incluido)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">superior a</td> 
   <td colspan="1" rowspan="1">Por encima del especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">menos que</td> 
   <td colspan="1" rowspan="1">Menor que el especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">al menos</td> 
   <td colspan="1" rowspan="1">Por encima del especificado (incluido)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">a lo sumo</td> 
   <td colspan="1" rowspan="1">Menor que el especificado (incluido)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">está vacío</td> 
   <td colspan="1" rowspan="1">Registros que no tienen valor (NULL): cero es un número, es <em>no</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no está vacío</td> 
   <td colspan="1" rowspan="1">Registros con CUALQUIER valor (incluido cero)</td> 
  </tr> 
 </tbody> 
</table>

Como puede ver, estos operadores facilitan hablar Marketo-ese con fluidez.
