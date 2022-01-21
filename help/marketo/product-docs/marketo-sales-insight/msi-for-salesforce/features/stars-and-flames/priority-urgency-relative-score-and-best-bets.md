---
unique-page-id: 2950396
description: 'Prioridad, urgencia, puntuación relativa y mejores mejoras: Marketo Docs: documentación del producto'
title: Prioridad, urgencia, puntuación relativa y mejores apuestas
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
source-git-commit: 15263f9c23c958499aaa2e4e6491b4962c617358
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Prioridad, urgencia, puntuación relativa y mejores apuestas {#priority-urgency-relative-score-and-best-bets}

Marketo Sales Insight elige los mejores posibles clientes y contactos según su prioridad. La prioridad de un posible cliente o contacto tiene dos componentes: urgencia y puntuación relativa.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Se derivan de la puntuación del posible cliente, una medida del interés de la persona en sus productos. Cuanto mayor sea la puntuación, más probabilidades habrá de que respondan positivamente a una llamada de su equipo de ventas.

>[!NOTE]
>
>Necesita varias campañas de puntuación para obtener el valor completo de prioridad, urgencia y puntuación relativa.  Con demasiadas campañas o sin puntuación, estos campos no serán útiles.

## Urgencia {#urgency}

Las llamas representan urgencia — cuánto ha cambiado recientemente la puntuación de plomo de esta persona. Una urgencia elevada (más llamas) significa que la puntuación de esta ventaja ha aumentado mucho últimamente; es una buena señal que este posible cliente esté interesado en su oferta. ¡Deberías seguirla con esta persona rápidamente!

Por ejemplo, un posible cliente que haya solicitado una demostración y haya visitado varias páginas web probablemente tenga una urgencia muy alta. Un posible cliente que no haya visitado su página web o abierto sus correos electrónicos tendrá una urgencia baja. Utilice la urgencia para priorizar quién debe ser contactado a continuación.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Puntaje relativo {#relative-score}

Las estrellas representan una puntuación relativa — una medida de cómo el puntaje inicial de esta persona se compara con el de todos los demás. Una puntuación relativa alta significa que esta persona probablemente esté más interesada e informada sobre su oferta en comparación con las personas con puntuaciones relativas inferiores.

Si dos posibles clientes tienen la misma urgencia, puede usar una puntuación relativa para saber cuál merece primero una llamada telefónica. El que tenga la puntuación relativa más alta puede reaccionar de forma más favorable a la oferta que el más bajo.

## Mejores apuestas {#best-bets}

Sus Mejores Apuestas son sus posibles clientes y contactos con la mayor urgencia y puntuación relativa. En esa lista solo están visibles los posibles clientes que posee y la lista se actualiza a medida que cambian las puntuaciones de los posibles clientes.

>[!NOTE]
>
>Si sus mejores apuestas no coinciden con los mejores posibles clientes y contactos que posee, hable con alguien de su empresa que tenga acceso a Marketo acerca de la actualización de su [Reglas de puntuación](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Cálculo de la urgencia y la puntuación relativa

Para calcular el número de estrellas y llamas, los posibles clientes y los contactos se ordenan primero por puntuación o cambio de puntuación (para Puntuación relativa y Urgencia, respectivamente). Luego se dividen en niveles: el nivel superior recibe la mayor cantidad de estrellas o llamas, el siguiente recibe menos, y así sucesivamente.

A medida que cambian las puntuaciones, se vuelven a calcular inmediatamente los valores de urgencia, prioridad y puntuación relativa. Los niveles de urgencia y puntuación relativa se calculan automáticamente cada noche en los servidores de Marketo.

>[!NOTE]
>
>Los recuentos de Urgencia relativa (llamas) y Puntuación relativa (estrellas) son números enteros en Marketo. Los valores posibles de cada uno son 0-3.
