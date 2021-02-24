---
unique-page-id: 7514146
description: Ejemplo de atribución 2 - Documentos de marketing - Documentación del producto
title: Ejemplo de atribución 2
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# Ejemplo de atribución 2 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* 11 de abril | La factura es adquirida por (feria comercial)
* 15 de abril | Joan es adquirida por (seminario web)
* 22 de abril | (Oportunidad 1) creada por $6.000
* 24 de abril | (Oportunidad 2) creada por 10.000 dólares
* 25 de abril | Bill y Joan están asociados con roles a **BOTH** Optys
* 29 de abril | (Oportunidad 1) es Closed-Won

| Nombre del programa | (Exposición comercial) | (Seminario web) |
|---|---|---|
| (FT) Opción creada | `<pre>1</pre>` | `<pre>1</pre>` |
| Canalización creada (FT) | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Ingresos obtenidos | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Dado que tanto Bill como Joan estuvieron asociados con roles a **AMBAS** oportunidades, el sistema (según las reglas) dividió el crédito de manera equitativa entre ellos.
>
>El oleoducto creado para cada programa (8.000 dólares) es la mitad del total (16.000 dólares) disponible como crédito.

>[!NOTE]
>
>**Reglas de atribución**
>
>1. El crédito se divide equitativamente
>1. No puedes dar más crédito del que ganaste
>1. No puedes dar crédito por algo que pasó en el pasado


Pruebe todos los ejemplos y usted será un profesional de atribución!

>[!MORELIKETHIS]
>
>* [Ejemplo de atribución 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Ejemplo de atribución 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Ejemplo de atribución 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

