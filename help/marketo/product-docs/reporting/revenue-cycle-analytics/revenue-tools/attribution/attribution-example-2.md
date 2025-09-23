---
unique-page-id: 7514146
description: 'Ejemplo de atribución 2: Documentos de Marketo: documentación del producto'
title: Ejemplo de atribución 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 7%

---

# Ejemplo de atribución 2 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* Abril de 11 | La factura la adquiere (feria comercial)
* Abril de 15 | Joan es adquirida por (seminario web)
* Abril de 22 | (Oportunidad 1) creada por 6.000 $
* Abril de 24 | (Oportunidad 2) creada por 10 000 $
* Abril de 25 | Bill y Joan están asociados con los roles de **BOTH** Optys
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
