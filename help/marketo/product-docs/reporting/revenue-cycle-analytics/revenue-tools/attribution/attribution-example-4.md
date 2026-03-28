---
unique-page-id: 7514151
description: Obtenga información acerca del ejemplo de atribución 4 en Marketo Engage, incluido el ejemplo de atribución 4. Utilice esta guía para completar el siguiente paso.
title: Ejemplo de atribución 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: f6893edbfe85d1d6e0958b5a3029d8fd404b1311
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 6%

---

# Ejemplo de atribución 4 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* Abril 11 | Michelle descarga libro electrónico (Contenido) - Éxito
* 15 de abril | John asiste (seminario web) - Éxito
* 22 de abril | (Oportunidad 1) creado para 3.000 $
* 24 de abril | (Oportunidad 2) creado por 5.000 $
* 25 de abril | John y Michelle están asociados a **ambas** opciones
* 29 de abril | La opción [Opty 1] está ganada

| Nombre del programa | (Contenido) | (Seminario web) | | |
|---|---|---|---|---|
|   | (Opción 1) | (Opción 2) | (Opción 1) | (Opción 2) |
| (MT) Opción creada | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Canal creado | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opción ganada | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Ingreso obtenido | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Cuando tiene varias oportunidades y varias personas con éxito en el programa, debe dividir el crédito entre las personas y los programas. Sin embargo, observe que el crédito por las oportunidades 1 y 2 no están combinadas. Cada una es una evaluación crediticia distinta.
>
>Cuando hay muchas personas involucradas, Marketo calculará automáticamente las fracciones de una oportunidad para dar crédito por.

>[!NOTE]
>
>**Reglas de atribución**
>
>1. El crédito se divide a partes iguales
>1. No puedes dar más crédito del que ganaste
>1. No puedes dar crédito por algo que pasó en el pasado

Pruebe todos los ejemplos y usted será un profesional de la atribución!

>[!MORELIKETHIS]
>
>* [Ejemplo de atribución 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Ejemplo de atribución 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Ejemplo de atribución 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
