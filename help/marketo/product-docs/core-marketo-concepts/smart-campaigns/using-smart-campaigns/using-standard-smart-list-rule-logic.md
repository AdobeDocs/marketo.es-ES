---
unique-page-id: 1147001
description: Uso de la lógica de regla de lista inteligente estándar - Documentos de Marketo - Documentación del producto
title: Uso de la lógica de regla de lista inteligente estándar
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Uso de la lógica de regla de lista inteligente estándar {#using-standard-smart-list-rule-logic}

Es posible que haya notado la opción &quot;Usar filtros&quot; al crear listas inteligentes de campañas. Esta configuración le permite decidir si los filtros deben evaluarse con un operador AND o OR .

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>El cambio de la lógica de reglas de lista inteligente solo se aplica a los filtros, **no** déclencheur.

Los déclencheur siempre se evalúan como O aunque la configuración anterior esté establecida en TODOS.  Este es un ejemplo:

![](assets/image2014-9-22-14-3a12-3a57.png)

La lista inteligente anterior con palabras:

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

Por lo tanto, si una persona rellena el formulario **o** visita la página, la campaña evaluará a esa persona en función de **todos** o **cualquiera** de los filtros siguientes, según la configuración utilizada.

>[!MORELIKETHIS]
>
>[Uso de la lógica de regla de lista inteligente avanzada](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
