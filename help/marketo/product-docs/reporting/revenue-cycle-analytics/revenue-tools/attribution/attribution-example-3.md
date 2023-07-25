---
unique-page-id: 7514149
description: 'Ejemplo de atribución 3: Documentos de Marketo: documentación del producto'
title: Ejemplo 3 de atribución
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Ejemplo 3 de atribución {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* Abril de 11 | Steve downloads (Contenido) - success
* Abril de 22 | Se crea una oportunidad por 3000 $ (tanto Steve como Jason tienen funciones)
* Abril de 25 | Jason asiste (seminario web) - success
* Abril de 30 | La oportunidad está cerrada-ganada

| Métrica de atribución | (Contenido) | (Seminario web) |
|---|---|---|
| (MT) Opción creada | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Canalización creada | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opción ganada | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Ingresos obtenidos | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Recordar #3 de reglas de atribución. Jason tuvo éxito en el programa DESPUÉS de que se creara la opción. Por lo tanto, el seminario web no puede obtener crédito por la creación de la oportunidad. Solo el crédito por el Opty ganó.
>
>Por lo tanto, (Contenido) tiene un 100% de crédito para la creación y canalización de Opty, pero solo un 50% de crédito para la opty ganada.

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
>* [Ejemplo 1 de atribución](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Ejemplo 2 de atribución](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Ejemplo 4 de atribución](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
