---
unique-page-id: 1147001
description: 'Uso de la lógica de regla de listas inteligentes estándar: Documentos de Marketo: documentación del producto'
title: Uso de la lógica de regla de listas inteligentes estándar
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Uso de la lógica de regla de listas inteligentes estándar {#using-standard-smart-list-rule-logic}

Es posible que haya visto la opción &quot;Usar filtros&quot; al crear listas inteligentes de campaña. Esta configuración le permite decidir si los filtros deben evaluarse con un operador AND u OR.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>El cambio de la lógica de reglas de listas inteligentes solo se aplica a filtros, **no** déclencheur.

Los déclencheur siempre se evalúan como O incluso si el ajuste anterior está establecido en TODO.  A continuación se muestra un ejemplo:

![](assets/image2014-9-22-14-3a12-3a57.png)

La lista inteligente anterior en palabras:

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

Por lo tanto, si una persona rellena el formulario **o** visita la página, la campaña evaluará a esa persona en función de **todo** o **cualquiera** de los filtros siguientes, según la configuración utilizada.

>[!MORELIKETHIS]
>
>[Uso de la lógica de regla de listas inteligentes avanzadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
