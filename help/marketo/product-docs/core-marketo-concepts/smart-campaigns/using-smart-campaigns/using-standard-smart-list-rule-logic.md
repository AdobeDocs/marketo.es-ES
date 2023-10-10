---
unique-page-id: 1147001
description: 'Uso de la lógica de regla de listas inteligentes estándar: Documentos de Marketo: documentación del producto'
title: Uso de la lógica de regla de listas inteligentes estándar
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 3916413a90e52a3423a8d7f78ad1c9eb45c2a219
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Uso de la lógica de regla de listas inteligentes estándar {#using-standard-smart-list-rule-logic}

Es posible que haya visto la opción &quot;Usar filtros&quot; al crear listas inteligentes de campaña. Esta configuración le permite decidir si los filtros deben evaluarse con un operador AND u OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>El cambio de la lógica de reglas de listas inteligentes solo se aplica a filtros, **no** déclencheur.

Los déclencheur siempre se evalúan como O incluso si el ajuste anterior está establecido en TODO. A continuación se muestra un ejemplo:

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

Por lo tanto, si una persona rellena el formulario **o** visita la página, la campaña evaluará a esa persona en función de **todo** o **cualquiera** de los filtros siguientes, según la configuración utilizada.

>[!MORELIKETHIS]
>
>[Uso de la lógica de regla de listas inteligentes avanzadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
