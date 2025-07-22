---
unique-page-id: 2950396
description: Prioridad, urgencia, puntuación relativa y recomendaciones - Documentos de Marketo - Documentación del producto
title: Prioridad, urgencia, puntuación relativa y resultados más probables
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Prioridad, urgencia, puntuación relativa y [!DNL Best Bets] {#priority-urgency-relative-score-and-best-bets}

[!DNL Marketo Sales Insight] elige a los mejores posibles clientes y contactos según su prioridad. La prioridad de un posible cliente o contacto tiene dos componentes: urgencia y puntuación relativa.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Se derivan de la puntuación del posible cliente, una medida del interés de la persona en sus productos. Cuanto más alta sea la puntuación, más probable es que respondan positivamente a una llamada de su equipo de ventas.

>[!NOTE]
>
>Necesita varias campañas de puntuación para obtener el valor completo de prioridad, urgencia y puntuación relativa.  Con muy pocas campañas de puntuación o ninguna, estos campos no serán útiles.

## Urgencia {#urgency}

Las llamas representan la urgencia, cuánto ha cambiado recientemente la puntuación de esta persona. Una alta urgencia (más llamas) significa que la puntuación de este posible cliente ha aumentado mucho últimamente; es una buena señal de que este posible cliente está interesado en su oferta. ¡Deberías seguir con esta persona rápidamente!

Por ejemplo, un posible cliente que solicitó una demostración y visitó varias páginas web probablemente tendrá una urgencia muy alta. Un posible cliente que no visitó su página web ni abrió sus correos electrónicos tendrá una baja urgencia. Utilice la urgencia para priorizar a quién se debe contactar a continuación.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Puntaje relativo {#relative-score}

Las estrellas representan una puntuación relativa; una medida de cómo se compara la puntuación de los posibles clientes de esta persona con la de todos los demás. Una puntuación relativa alta significa que esta persona está probablemente más interesada e informada sobre su oferta en comparación con las personas con puntuaciones relativas más bajas.

Si dos posibles clientes tienen la misma urgencia, puede usar una puntuación relativa para saber cuál merece una llamada telefónica primero. El que tenga la puntuación relativa más alta puede reaccionar más favorablemente a su oferta en comparación con la más baja.

## [!DNL Best Bets] {#best-bets}

Sus [!DNL Best Bets] son sus posibles clientes y contactos con la mayor urgencia y puntuación relativa. Solo los posibles clientes que posea serán visibles en esa lista y esta se actualizará a medida que cambien las puntuaciones de los posibles clientes.

>[!NOTE]
>
>Si tus mejores resultados no coinciden con los mejores posibles clientes y contactos que tienes, habla con alguien de tu empresa que tenga acceso a Marketo para actualizar tus [reglas de puntuación](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Cómo se calculan la urgencia y la puntuación relativa

Para calcular el número de estrellas y llamas, los posibles clientes y contactos se ordenan primero por puntuación o cambio de puntuación (para Puntuación relativa y Urgencia, respectivamente). Luego se dividen en niveles: el nivel superior recibe la mayor cantidad de estrellas o llamas, el siguiente recibe menos, y así sucesivamente.

A medida que cambian las puntuaciones, los valores de urgencia, prioridad y puntuación relativa se vuelven a calcular inmediatamente. Los niveles de urgencia y de puntuación relativa se calculan automáticamente cada noche en los servidores de Marketo.

>[!NOTE]
>
>Los recuentos Relative Urgency (llamas) y Relative Score (estrellas) son enteros en Marketo. Los valores posibles para cada uno son de 0 a 3.
