---
unique-page-id: 7514126
description: 'Ejemplo de atribución 1: Documentos de Marketo: documentación del producto'
title: Ejemplo 1 de atribución
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 4%

---

# Ejemplo 1 de atribución {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* Abril de 11 | Fred es adquirido por (Tradeshow)
* Abril de 15 | Margo asiste (seminario web) - success
* Abril de 22 | Fred está asociado (función) a la oportunidad
* Abril de 22 | Se ha creado la oportunidad por 3000 $

| Nombre del programa | (Feria) | (Seminario web) |
|---|---|---|
| (FT) Opción creada | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Canal creado | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Ingreso obtenido | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>En primer lugar, es comprender que algunos tipos son CONTADORES y otros MONEDA. La opción Creada es un recuento, un número entero. La canalización es una moneda. En Marketo, la divisa se ajustará a la configuración de la configuración regional del administrador.
>
>La razón por la que la Feria recibió todo el crédito es porque Margo no estaba asociado con un rol en la oportunidad. Sin papel, sin crédito.

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
>* [Ejemplo de atribución 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Ejemplo de atribución 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Ejemplo de atribución 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
