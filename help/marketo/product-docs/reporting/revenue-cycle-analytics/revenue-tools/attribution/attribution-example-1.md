---
unique-page-id: 7514126
description: Ejemplo de atribución 1 - Documentos de Marketo - Documentación del producto
title: Ejemplo de atribución 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%

---

# Ejemplo de atribución 1 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* 11 de abril | Fred es adquirido por (feria comercial)
* 15 de abril | Asistentes de Margo (seminario web): éxito
* 22 de abril | Fred está asociado (rol) a la oportunidad
* 22 de abril | La oportunidad se crea por 3.000 dólares

| Nombre del programa | (Exposición comercial) | (Seminario web) |
|---|---|---|
| (FT) Opción creada | `<pre>1</pre>` | `<pre>0</pre>` |
| Canalización creada (FT) | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Ganancias | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Primero es comprender que algunos tipos son RECUENTO y otros son MONEDA. Opty Created es un recuento, un número entero. La canalización es una moneda. En Marketo, la moneda se ajustará a la configuración regional de administración.
>
>La razón por la que la feria recibió todo el crédito es porque Margo no estaba asociado con un rol en la oportunidad. Sin rol, sin crédito.

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
>* [Ejemplo de atribución 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Ejemplo de atribución 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Ejemplo de atribución 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

