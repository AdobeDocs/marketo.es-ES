---
unique-page-id: 7514146
description: Obtenga información acerca del ejemplo de atribución 2 en Marketo Engage, incluido el ejemplo de atribución 2 ejemplo de atribución. Utilice esta guía para completar el siguiente paso.
title: Ejemplo de atribución 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 126e34f9-e02a-505e-9978-ea36537f3ef9
    internal-label: Revenue Cycle Analytics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 7%
---
# Ejemplo de atribución 2 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* Abril de 11 | Bill es adquirido por (Feria)
* Abril de 15 | Joan es adquirida por (Seminario web)
* Abril de 22 | (Oportunidad 1) creado por 6.000 $
* Abril de 24 | (Oportunidad 2) creado por 10 000 $
* Abril de 25 | Bill y Joan están asociados con roles a **BOTH** Optys
* Abril de 29 | (Oportunidad 1) está Cerrada-Ganada

| Nombre del programa | (Feria) | (Seminario web) |
|---|---|---|
| (FT) Opción creada | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Canal creado | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Ingreso obtenido | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Dado que Bill y Joan estaban asociados con roles a **AMBAS** oportunidades, el sistema (según las reglas) dividió el crédito de manera uniforme entre ellos.
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
>* [Ejemplo de atribución 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Ejemplo de atribución 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Ejemplo de atribución 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
