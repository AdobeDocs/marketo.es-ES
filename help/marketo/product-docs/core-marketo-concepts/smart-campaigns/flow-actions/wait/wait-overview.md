---
unique-page-id: 1146950
description: 'Esperar: documentos de Marketo: documentación del producto'
title: Esperar
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Esperar {#wait}

## Información general {#overview}

Pausar a una persona en un flujo de campaña inteligente con la práctica **paso de espera**.

![](assets/wait-overview.png)

Observe cómo puede escribir en lenguaje natural como &quot;4 horas&quot;. Hacer **no**, sin embargo, abreviar las palabras (es decir, 4 horas). La campaña inteligente seguiría ejecutándose, pero el paso de espera se ignoraría.

>[!CAUTION]
>
>Cambiar la duración de un paso de espera no afectará a las personas que ya lo hayan ingresado. Por ejemplo: tiene un paso de espera de 5 días, una persona lo introduce y, a continuación, cambia el paso de espera a 7 días: esa persona solo esperará los 5 días originales antes de avanzar al siguiente paso de flujo.

>[!TIP]
>
>Si ya tiene a alguien en un paso de espera y no desea que avance después de que finalice el período de espera, inserte [quitar del flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) justo después del paso de espera. Especifique a quién desea eliminar mediante el [añadir opción](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) opción.

## Uso {#usage}

Existen tres formas principales de utilizar un paso de flujo de espera:

1. [Utilizar una duración en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Usar una fecha específica en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Uso de un token de fecha en un paso de flujo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
