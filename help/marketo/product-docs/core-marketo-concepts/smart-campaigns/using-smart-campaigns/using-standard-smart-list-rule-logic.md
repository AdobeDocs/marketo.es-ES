---
unique-page-id: 1147001
description: Aprenda a utilizar la lógica de regla de listas inteligentes estándar en una campaña inteligente. Combine filtros con la lógica AND para la calificación.
title: Uso de la lógica de regla de listas inteligentes estándar
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/hRPdzjEUOeC2PZK2YlO1IPZOPoPOfo7CHJu2yUtU0qc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 10%

---

# Uso de la lógica de regla de listas inteligentes estándar {#using-standard-smart-list-rule-logic}

Es posible que haya visto la opción &quot;Usar filtros&quot; al crear listas inteligentes de campaña. Esta configuración le permite decidir si los filtros deben evaluarse con un operador AND u OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>El cambio de la lógica de reglas de listas inteligentes solo se aplica a los déclencheur, _no_.

Los déclencheur siempre se evalúan como O incluso si el ajuste anterior está establecido en TODO. Por ejemplo:

![](assets/using-standard-smart-list-rule-logic-2.png)

La lista inteligente anterior en palabras:

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page
AND
Industry is Energy
AND
Country is US
THEN follow the campaign's flow step(s)
```

Por lo tanto, si una persona rellena el formulario _o_ visita la página, la campaña evaluará a esa persona en función de _todos_ o _cualquiera_ de los filtros subsiguientes, según la configuración utilizada.

>[!MORELIKETHIS]
>
>[Usando lógica avanzada de reglas de listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
