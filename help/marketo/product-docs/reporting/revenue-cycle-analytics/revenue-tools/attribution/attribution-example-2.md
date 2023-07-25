---
unique-page-id: 7514146
description: 'Ejemplo de atribución 2: Documentos de Marketo: documentación del producto'
title: Ejemplo 2 de atribución
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 2%

---

# Ejemplo 2 de atribución {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* Abril de 11 | Bill es adquirido por (Feria)
* Abril de 15 | Joan es adquirida por (Seminario web)
* Abril de 22 | (Oportunidad 1) creado por 6.000 $
* Abril de 24 | (Oportunidad 2) creado por 10 000 $
* Abril de 25 | Bill y Joan están asociados con roles a **AMBOS** Optys
* Abril de 29 | (Oportunidad 1) está Cerrada-Ganada

| Nombre del programa | (Exposición comercial) | (Seminario web) |
|---|---|---|
| (FT) Opción creada | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Canalización creada | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Ingresos obtenidos | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Porque Bill y Joan estaban asociados con roles de **AMBOS** oportunidades, el sistema (de acuerdo con las reglas) dividió el crédito uniformemente entre ellas.
>
>La canalización creada para cada programa (8.000 dólares) es la mitad del total (16.000 dólares) disponible para dar como crédito.

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
>* [Ejemplo 3 de atribución](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Ejemplo 4 de atribución](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
