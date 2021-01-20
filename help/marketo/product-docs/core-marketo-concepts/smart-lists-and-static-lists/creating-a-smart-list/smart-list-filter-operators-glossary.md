---
unique-page-id: 557312
description: Glosario de operadores de filtros de Lista inteligente - Documentos de marketing - Documentación del producto
title: Glosario de operadores de filtros de Lista inteligente
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---


# Glosario de operadores de filtros de Lista inteligente {#smart-list-filter-operators-glossary}

Un operador es una parte de la lista inteligente que le ayuda a ser específico. Permite describir el filtro o el déclencheur en lenguaje sencillo. Los operadores disponibles son diferentes para cada tipo de campo.

Aquí hay un glosario que describe cada conjunto de operadores.

## Campos de fecha {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Al elegir un operador, el lado derecho cambiará dinámicamente.

| Operador | Lado derecho | Descripción |
|---|---|---|
| is | Fecha única | Coincidencia de fecha exacta |
| no es | Fecha única | Cualquier fecha EXCEPTO la especificada |
| entre | Dos campos de fecha | Cualquier fecha que incluya y entre dos fechas especificadas |
| en el pasado | Entrada de lenguaje natural* | Consulte el diagrama siguiente |
| en el pasado antes | Entrada de lenguaje natural* | Consulte el diagrama siguiente |
| en el futuro | Entrada de lenguaje natural* | Consulte el diagrama siguiente |
| en el futuro después de | Entrada de lenguaje natural* | Consulte el diagrama siguiente |
| en el lapso de tiempo | Ajustes preestablecidos (último trimestre, ayer, etc.) | Definido en la lista de selección |
| after | Fecha única | Todos los registros posteriores a la fecha especificada |
| before | Fecha única | Todos los registros anteriores al especificado |
| en o después | Fecha única | Igual que &quot;después&quot; pero inclusivo |
| en o antes | Fecha única | Igual que &quot;antes&quot; pero inclusivo |
| está vacío | Ninguno | Todos los registros sin fecha |
| no está vacío | Ninguno | Todos los registros con cualquier fecha |

* La entrada de lenguaje natural es genial. Estos son algunos de los patrones que puede introducir:

* 1 hora
* 82 días
* 3 semanas
* 14 meses
* 1 año

Solo tiene que escribir el número y la unidad juntos y funcionará.

>[!NOTE]
>
>&quot;Anteriormente&quot; **incluye** el día (hasta el momento, no después) que se crea la lista inteligente.

>[!CAUTION]
>
>Cuando crea una lista inteligente con un filtro de campo de fecha (por ejemplo, Fecha de nacimiento, Fecha de creación de SFDC) y utiliza las restricciones **antes** o **antes o antes de**, la lista inteligente también incluirá personas que no tengan valor en dicho campo de fecha.

Utilice el diagrama siguiente para comprender la diferencia entre los operadores de fecha.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Ejemplo**
>
>Los campos de fecha pueden complicarse cuando se trabaja con eventos pasados y futuros. Aquí hay un par de ejemplos.
>
>**En el pasado antes**
>
>Para la nueva promoción, utilice este operador para enviar correos electrónicos únicamente a las personas que no se hayan suscrito o renovado el servicio en el plazo de un año o que nunca hayan sido suscriptores.
>
>**En el futuro, después de**
>
>Si desea ver a los clientes que están disponibles para la renovación en 90 días. Usaría dos filtros separados. Primero utilice &quot;En el futuro después de 90 días&quot; y segundo, &quot;En el futuro 91 días&quot;. Eso capturaría a quien tenga una fecha dentro de 90 días.

## Campos de cadena {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operador | Descripción |
|---|---|
| is | Coincidencia exacta (no distingue entre mayúsculas y minúsculas) |
| no es | Cualquiera EXCEPTO coincidencia exacta |
| inicios con | Primeras letras de coincidencia de cadena |
| no inicios con | Las primeras letras de la cadena NO coinciden |
| contains | Coinciden todas las letras de la cadena (ejemplo: california, fortuna, por ahí) |
| no contiene | No hay letras juntas en la coincidencia de cadena. (reverso de &quot;contains&quot;) |
| está vacío | Registros que no tienen valor (NULL) |
| no está vacío | Registros con valor CUALQUIER |

>[!TIP]
>
>Utilice operadores positivos sobre negativos. Los filtros &quot;no es&quot; tienen que buscar en todo el conjunto de datos de la instancia, lo que puede llevar mucho tiempo. Los filtros &quot;is&quot; positivos pueden aprovechar algoritmos de búsqueda más eficaces.

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
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">Coincidencia de número exacta ( = 0 devolverá ambos leads con 0 <em>y</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no es</td> 
   <td colspan="1" rowspan="1">Cualquiera EXCEPTO coincidencia de número exacto</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">entre</td> 
   <td colspan="1" rowspan="1">Defina dos valores para encontrar a todos los que se encuentran entre ambos (incluido)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">bueno que</td> 
   <td colspan="1" rowspan="1">Por encima del valor especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">menor que</td> 
   <td colspan="1" rowspan="1">Menor que el especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">al menos</td> 
   <td colspan="1" rowspan="1">Por encima del especificado (incluido)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">como máximo</td> 
   <td colspan="1" rowspan="1">Menor que el especificado (incluido)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">está vacío</td> 
   <td colspan="1" rowspan="1">Registros que no tienen valor (NULL): cero es un número, es <em>no</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no está vacío</td> 
   <td colspan="1" rowspan="1">Registros con valor CUALQUIER (incluyendo cero)</td> 
  </tr> 
 </tbody> 
</table>

Como pueden ver, estos operadores hacen que sea fácil hablar el marketo-ese con fluidez!
