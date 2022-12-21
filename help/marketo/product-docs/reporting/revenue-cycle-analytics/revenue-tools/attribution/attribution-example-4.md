---
unique-page-id: 7514151
description: Ejemplo de atribución 4 - Documentos de Marketo - Documentación del producto
title: Ejemplo de atribución 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 2%

---

# Ejemplo de atribución 4 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* 11 de abril | Michelle descarga e-Book (contenido) - Éxito
* 15 de abril | John asiste (seminario web): éxito
* 22 de abril | (Oportunidad 1) creada por 3.000 dólares
* 24 de abril | (Oportunidad 2) creada por 5.000 dólares
* 25 de abril | John y Michelle están asociados a **both** Optys
* 29 de abril | [Opt 1] es Cerrado-Ganado

| Nombre del programa | (Contenido) | (Seminario web) |
|---|---|---|
|  | (Opty 1) | (Opty 2) | (Opty 1) | (Opty 2) |
| (MT) Opción creada | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| Canalización creada (MT) | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Ganancias | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Cuando tiene múltiples oportunidades y varias personas con éxito en el programa, debe dividir el crédito entre las personas y los programas. Sin embargo, observe que el crédito por las oportunidades 1 y 2 no se combina. Cada una es una evaluación de crédito distinta.
>
>Cuando intervienen muchas personas, Marketo calculará automáticamente las fracciones de una oportunidad para dar crédito.

>[!NOTE]
>
>**Reglas de atribución**
>
>1. El crédito se divide a partes iguales
>1. No puedes dar más crédito del que ganaste
>1. No puedes dar crédito por algo que pasó en el pasado


Pruebe todos los ejemplos y será un profesional de la atribución!

>[!MORELIKETHIS]
>
>* [Ejemplo de atribución 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Ejemplo de atribución 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Ejemplo de atribución 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

