---
unique-page-id: 7514149
description: Ejemplo de atribución 3 - Marketo Docs - Documentación del producto
title: Ejemplo de atribución 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Ejemplo de atribución 3 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* 11 de abril | Steve downloads (Content) - success
* 22 de abril | La oportunidad se crea para $3,000 (Steve y Jason tienen roles)
* 25 de abril | Jason asiste (seminario web): éxito
* 30 de abril | La oportunidad está cerrada

| Métrica de atribución | (Contenido) | (Seminario web) |
|---|---|---|
| (MT) Opción creada | `<pre>1</pre>` | `<pre>0</pre>` |
| Canalización creada (MT) | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Ganancias | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Recuerde la regla de atribución n.º 3. Jason tuvo éxito en el programa DESPUÉS de que se creara la posta. Por lo tanto, el seminario web no puede obtener crédito por la creación de la oportunidad. Solamente el crédito por el Opty ganó.
>
>Por lo tanto, (Contenido) tiene el 100% del crédito por la creación y canalización de Opty, pero solo el 50% del crédito por la posta ganó.

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
>* [Ejemplo de atribución 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

