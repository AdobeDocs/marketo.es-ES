---
unique-page-id: 1146950
description: 'Espera: Documentos de Marketo: documentación del producto'
title: Esperar
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Esperar {#wait}

## Resumen {#overview}

Poner en pausa a una persona en un flujo de campaña inteligente con lo práctico **paso de espera**.

![](assets/wait-overview.png)

Observe cómo puede escribir en un lenguaje natural como &quot;4 horas&quot;. Do **not**, sin embargo, abreviar las palabras (es decir, 4 horas). La campaña inteligente seguiría ejecutándose, pero el paso de espera se ignoraría.

>[!CAUTION]
>
>Cambiar la duración de un paso de espera no afectará a las personas que ya lo hayan introducido. Por ejemplo: Si tiene un paso de espera durante 5 días, una persona lo introduce y luego cambia el paso de espera a 7 días, esa persona solo esperará los 5 días originales antes de pasar al siguiente paso de flujo.

>[!TIP]
>
>Si ya tiene a alguien en un paso de espera y no desea que avance después de que termine el período de espera, inserte [eliminar del flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) justo después del paso de espera. Especifique a quién desea eliminar utilizando la variable [añadir opción](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) .

## Uso {#usage}

Existen tres formas principales de utilizar un paso de flujo de espera:

1. [Usar una duración en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Uso de un token de fecha en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
