---
unique-page-id: 1147001
description: Uso de la lógica de reglas de Lista inteligente estándar - Documentos de marketing - Documentación del producto
title: Uso de la lógica de regla de Lista inteligente estándar
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# Uso de la lógica de regla de Lista inteligente estándar {#using-standard-smart-list-rule-logic}

Es posible que haya notado la opción &quot;Usar filtros&quot; al crear listas inteligentes de campaña. Esta configuración le permite decidir si los filtros deben evaluarse con un operador Y o O.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>El cambio de la lógica de reglas de lista inteligente solo se aplica a filtros, **no** déclencheur.

Los déclencheur siempre se evalúan como O aunque la configuración anterior esté establecida en TODOS.  A continuación se muestra un ejemplo:

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

Por lo tanto, si una persona rellena el formulario **o** visita la página, la campaña luego evaluará a esa persona en base a **todo** o **cualquiera** de los filtros subsiguientes, según la configuración utilizada.

>[!MORELIKETHIS]
>
>[Uso de la lógica avanzada de reglas de Lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
