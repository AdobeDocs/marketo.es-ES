---
unique-page-id: 557312
description: Glosario de operadores de filtros de listas inteligentes - Documentos de Marketo - Documentación del producto
title: Glosario de operadores de filtros de listas inteligentes
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 13%

---

# Glosario de operadores de filtros de listas inteligentes {#smart-list-filter-operators-glossary}

Un operador es una parte de la lista inteligente que le ayuda a obtener permisos específicos. Permite describir el filtro o déclencheur en un lenguaje sencillo. Los operadores disponibles son diferentes para cada tipo de campo.

Este glosario describe cada conjunto de operadores.

## Campos de fecha {#date-fields}

![](assets/smart-list-filter-operators-glossary-1.png)

Al elegir un operador, el lado derecho cambia de forma dinámica.

<table><thead>
  <tr>
    <th>Operador</th>
    <th>Lado derecho</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>es/está</td>
    <td>Fecha única</td>
    <td>Coincidencia de fecha exacta</td>
  </tr>
  <tr>
    <td>no es/no está</td>
    <td>Fecha única</td>
    <td>Cualquier fecha excepto la especificada</td>
  </tr>
  <tr>
    <td>entre</td>
    <td>Dos campos de fecha</td>
    <td>Cualquier fecha, incluidas y entre dos fechas especificadas</td>
  </tr>
  <tr>
    <td>en el anterior</td>
    <td>Entrada de lenguaje natural*</td>
    <td>Consulte el diagrama siguiente</td>
  </tr>
  <tr>
    <td>en el pasado anterior</td>
    <td>Entrada de lenguaje natural*</td>
    <td>Consulte el diagrama siguiente</td>
  </tr>
  <tr>
    <td>en el futuro</td>
    <td>Entrada de lenguaje natural*</td>
    <td>Consulte el diagrama siguiente</td>
  </tr>
  <tr>
    <td>en el futuro posterior</td>
    <td>Entrada de lenguaje natural*</td>
    <td>Consulte el diagrama siguiente</td>
  </tr>
  <tr>
    <td>en el marco temporal</td>
    <td>Ajustes preestablecidos (último trimestre, ayer, etc.)</td>
    <td>Definido en la lista de selección</td>
  </tr>
  <tr>
    <td>después</td>
    <td>Fecha única</td>
    <td>Todos los registros posteriores a la fecha especificada</td>
  </tr>
  <tr>
    <td>antes</td>
    <td>Fecha única</td>
    <td>Todos los registros anteriores al especificado</td>
  </tr>
  <tr>
    <td>el o después</td>
    <td>Fecha única</td>
    <td>Igual que "después", pero inclusivo</td>
  </tr>
  <tr>
    <td>el o antes del</td>
    <td>Fecha única</td>
    <td>Igual que "antes" pero inclusivo</td>
  </tr>
  <tr>
    <td>está vacío</td>
    <td>Ninguno</td>
    <td>Todos los registros sin fecha</td>
  </tr>
  <tr>
    <td>no está vacío</td>
    <td>Ninguno</td>
    <td>Todos los registros con cualquier fecha</td>
  </tr>
</tbody></table>

**&#42;**: la entrada en lenguaje natural es genial. Estos son algunos de los patrones que puede introducir:

* 1 hora
* 82 días
* 3 semanas
* 14 meses
* 1 año

Solo escribe el número y la unidad juntos y va a funcionar!

>[!NOTE]
>
>&quot;En el pasado&quot; _sí_ incluye el día (hasta el momento, no después) en que crea su lista inteligente.

>[!CAUTION]
>
>Cuando crea una lista inteligente usando un filtro de campo de fecha (por ejemplo, Fecha de nacimiento, Fecha de creación de SFDC) y usa las restricciones **[!UICONTROL antes de]**, **[!UICONTROL en o antes de]**, o **[!UICONTROL en el pasado antes de]**, la lista inteligente también incluirá a las personas que no tienen valor en dicho campo de fecha.

Utilice el diagrama siguiente para comprender la diferencia entre los operadores de fecha.

![](assets/smart-list-filter-operators-glossary-2.png)

>[!NOTE]
>
>**Ejemplo**
>
>Los campos de fecha pueden resultar complicados cuando se trabaja con eventos pasados y futuros. Aquí hay un par de ejemplos.
>
>**[!UICONTROL Anterior a]**
>
>Para la nueva promoción, utilice este operador para enviar correos electrónicos solo a las personas que no se hayan suscrito o renovado el servicio en el plazo de un año o que nunca se hayan suscrito.
>
>**[!UICONTROL En el futuro después de]**
>
>Supongamos que desea ver los clientes que se van a renovar en 90 días. Se utilizan dos filtros independientes. Primero use &quot;En el futuro después de 90 días&quot; y segundo, &quot;En el futuro en 91 días&quot;. Eso capturaría a quien tenga una cita dentro de 90 días.

## Campos de cadena {#string-fields}

![](assets/smart-list-filter-operators-glossary-3.png)

<table><thead>
  <tr>
    <th>Operador</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>es/está</td>
    <td>Coincidencia exacta (sin distinción de mayúsculas y minúsculas)</td>
  </tr>
  <tr>
    <td>no es/no está</td>
    <td>Cualquier cosa excepto coincidencia exacta</td>
  </tr>
  <tr>
    <td>comienza con</td>
    <td>Coincidencia de las primeras letras de la cadena</td>
  </tr>
  <tr>
    <td>no comienza con</td>
    <td>Las primeras letras de la cadena NO coinciden</td>
  </tr>
  <tr>
    <td>contiene</td>
    <td>Cualquier letra de la cadena coincide (por ejemplo: california, queue, etc.)</td>
  </tr>
  <tr>
    <td>no contiene</td>
    <td>No hay letras juntas en la cadena que coincidan. (al revés de "contiene")</td>
  </tr>
  <tr>
    <td>está vacío</td>
    <td>Registros sin valor (NULL)</td>
  </tr>
  <tr>
    <td>no está vacío</td>
    <td>Registros con valor ANY</td>
  </tr>
</tbody>
</table>

>[!TIP]
>
>Utilice operadores positivos sobre negativos. Los filtros &quot;No es&quot; tienen que buscar todo el conjunto de datos en su instancia, lo que puede consumir mucho tiempo. Los filtros positivos &quot;es&quot; pueden aprovechar algoritmos de búsqueda más eficaces.

## Campos enteros {#integer-fields}

![](assets/smart-list-filter-operators-glossary-4.png)

<table><thead>
  <tr>
    <th>Operador</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>es/está</td>
    <td>La coincidencia de número exacto ( = 0 devolverá ambos posibles clientes con 0 y NULL)</td>
  </tr>
  <tr>
    <td>no es/no está</td>
    <td>Cualquier cosa EXCEPTO el número exacto coincide</td>
  </tr>
  <tr>
    <td>entre</td>
    <td>Defina dos valores para encontrar a todos los que estén en el medio (incluido)</td>
  </tr>
  <tr>
    <td>más que</td>
    <td>Por encima del especificado</td>
  </tr>
  <tr>
    <td>menos que</td>
    <td>Menor que el especificado</td>
  </tr>
  <tr>
    <td>al menos</td>
    <td>Por encima del especificado (incluido)</td>
  </tr>
  <tr>
    <td>a lo sumo</td>
    <td>Menor que el especificado (incluido)</td>
  </tr>
  <tr>
    <td>está vacío</td>
    <td>Registros sin valor (NULL): cero es un número, no es NULL</td>
  </tr>
  <tr>
    <td>no está vacío</td>
    <td>Registros con CUALQUIER valor (incluido cero)</td>
  </tr>
</tbody>
</table>

Como puede ver, estos operadores facilitan hablar Marketo-ese con fluidez.
