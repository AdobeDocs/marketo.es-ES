---
unique-page-id: 557312
description: Glosario de operadores de filtros de lista inteligente - Documentos de Marketo - Documentación del producto
title: Glosario de operadores de filtros de lista inteligente
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Glosario de operadores de filtros de lista inteligente {#smart-list-filter-operators-glossary}

Un operador es una parte de la lista inteligente que le ayuda a obtener información específica. Permite describir el filtro o el déclencheur en lenguaje directo. Los operadores disponibles son diferentes para cada tipo de campo.

Aquí hay un glosario que describe cada conjunto de operadores.

## Campos de fecha {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Al elegir un operador, el lado derecho cambiará dinámicamente.

| Operador | Lado derecho | Descripción |
|---|---|---|
| es | Fecha única | Coincidencia de fecha exacta |
| no es | Fecha única | Cualquier fecha EXCEPTO la especificada |
| entre | Dos campos de fecha | Cualquier fecha que incluya y entre dos fechas especificadas |
| en el pasado | Entrada de idioma natural* | Consulte el diagrama siguiente |
| en versiones anteriores | Entrada de idioma natural* | Consulte el diagrama siguiente |
| en el futuro | Entrada de idioma natural* | Consulte el diagrama siguiente |
| en el futuro después de | Entrada de idioma natural* | Consulte el diagrama siguiente |
| en tiempo de espera | Ajustes preestablecidos (último trimestre, ayer, etc.) | Definido en la lista de selección |
| after | Fecha única | Todos los registros posteriores a la fecha especificada |
| before | Fecha única | Todos los registros anteriores al especificado |
| en o después | Fecha única | Igual que &quot;después&quot; pero inclusivo |
| en o antes | Fecha única | Igual que &quot;before&quot; pero inclusivo |
| está vacío | Ninguna | Todos los registros sin fecha |
| no está vacío | Ninguna | Todos los registros con cualquier fecha |

* La entrada de lenguaje natural es genial. Estos son algunos de los patrones que puede introducir:

* 1 hora
* 82 días
* 3 semanas
* 14 meses
* 1 año

Solo tiene que escribir el número y la unidad juntos y funcionará.

>[!NOTE]
>
>&quot;En el pasado&quot; **sí** incluye el día (hasta la hora, no después) que crea la lista inteligente.

>[!CAUTION]
>
>Cuando crea una lista inteligente con un filtro de campo de fecha (por ejemplo, Fecha de nacimiento, Fecha de creación de SFDC) y utiliza las restricciones **before** o **on or before** , la lista inteligente también incluye personas que no tienen valor en ese campo de fecha.

Utilice el diagrama siguiente para comprender la diferencia entre los operadores de fecha.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Ejemplo**
>
>Los campos de fecha pueden resultar complicados cuando se trabaja con eventos pasados y futuros. Aquí hay un par de ejemplos.
>
>**En el pasado**
>
>Para la nueva promoción, utilice este operador para enviar correos electrónicos solo a las personas que no se hayan suscrito o renovado el servicio en el plazo de un año o que nunca hayan sido suscriptores.
>
>**En el futuro, después**
>
>Supongamos que desea ver a los clientes que pueden renovarse en 90 días. Se usarían dos filtros independientes. En primer lugar utilice &quot;En el futuro después de 90 días&quot; y en segundo lugar, &quot;En el futuro durante 91 días&quot;. Eso capturaría a quien tenga una fecha dentro de 90 días.

## Campos de cadena {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operador | Descripción |
|---|---|
| es | Coincidencia exacta (sin distinción de mayúsculas y minúsculas) |
| no es | Cualquier coincidencia EXCEPTO exacta |
| comienza con | Primeras letras de coincidencia de cadena |
| no comienza con | Las primeras letras de la cadena NO coinciden |
| contains | Cualquier letra junto en la cadena coincide (ejemplo: california, fortuna, por ahí) |
| not contains | No hay letras juntas en la cadena que coincidan. (reverso de &quot;contiene&quot;) |
| está vacío | Registros que no tienen valor (NULL) |
| no está vacío | Registros con cualquier valor |

>[!TIP]
>
>Utilice operadores positivos sobre negativos. Los filtros &quot;No es&quot; tienen que buscar todo el conjunto de datos de su instancia, lo que puede consumir mucho tiempo. Los filtros &quot;is&quot; positivos pueden aprovechar algoritmos de búsqueda más eficaces.

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
   <td colspan="1" rowspan="1">Coincidencia de número exacta ( = 0 devolverá ambos posibles clientes con 0 <em>y</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no es</td> 
   <td colspan="1" rowspan="1">Cualquier coincidencia EXCEPTO el número exacto</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">entre</td> 
   <td colspan="1" rowspan="1">Defina dos valores para encontrar a todos los que se encuentran entre medias (incluido)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">bueno que</td> 
   <td colspan="1" rowspan="1">Sobre el especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">menor que</td> 
   <td colspan="1" rowspan="1">Menor que el especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">al menos</td> 
   <td colspan="1" rowspan="1">Sobre el especificado (incluido)</td> 
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
   <td colspan="1" rowspan="1">Registros con CUALQUIER valor (incluido cero)</td> 
  </tr> 
 </tbody> 
</table>

Como pueden ver, estos operadores hacen que sea fácil hablar Marketo-ese con fluidez!
