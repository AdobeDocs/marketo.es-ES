---
unique-page-id: 1146901
description: Uso de la lógica de regla de listas inteligentes avanzada - Documentos de Marketo - Documentación del producto
title: Uso de la lógica de regla de listas inteligentes avanzadas
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: d087b22e84c23fea5e38fe7bf20349dc7eec09f7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Uso de la lógica de regla de listas inteligentes avanzadas {#using-advanced-smart-list-rule-logic}

Puede encontrar exactamente las personas que necesita aplicando la lógica de regla de listas inteligentes a varios filtros dentro de una lista inteligente. Así es como.

>[!PREREQUISITES]
>
>* [Buscar y agregar filtros a una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}
>* [Definir filtros de listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md){target="_blank"}

>[!NOTE]
>
>La lógica de filtro avanzada solo está disponible si hay tres o más filtros en la lista inteligente.

## Agregar lógica a una lista inteligente {#add-logic-to-a-smart-list}

De forma predeterminada, la lista inteligente encontrará las personas que coinciden con los filtros **[!UICONTROL ALL]** (filtros 1 _y_ 2 _y_ 3). Puede cambiar la lógica de la regla para buscar personas que coincidan con **[!UICONTROL ANY]** de los filtros definidos (filtros 1 _o_ 2 _o_ 3), o usar filtros avanzados (filtros 1 _y_ 2 _o_ 3).

En este ejemplo, supongamos que desea buscar personas en California _y_ con una puntuación de al menos 50 puntos _o_ con el estado &quot;Ventas calificadas&quot;.

1. Seleccione **[!UICONTROL Usar filtros avanzados]** en la lista desplegable.

   ![](assets/using-advanced-smart-list-rule-logic-1.png)

   >[!NOTE]
   >
   >El uso de filtros **[!UICONTROL Avanzados]** reduce la necesidad de crear listas inteligentes con el filtro Miembro de lista inteligente. Esto ayuda a optimizar el rendimiento.

1. El cuadro de texto **[!UICONTROL Filtros avanzados]** mostrará &quot;y&quot; como el valor predeterminado entre todos los filtros.

   ![](assets/using-advanced-smart-list-rule-logic-2.png)

1. Escriba un par de paréntesis alrededor de &quot;2 y 3&quot;.

   ![](assets/using-advanced-smart-list-rule-logic-3.png)

   >[!CAUTION]
   >
   >Debe utilizar &quot;y&quot; antes de &quot;o&quot; al introducir la lógica de regla.

1. Cambie &quot;and&quot; entre &quot;2 y 3&quot; y &quot;or&quot;.

   ![](assets/using-advanced-smart-list-rule-logic-4.png)

## Utilice Paréntesis Al Combinar &quot;And&quot; Y &quot;Or {#use-parentheses-when-mixing-and-and-or}

La combinación de las lógicas &quot;and&quot; y &quot;or&quot; requiere paréntesis para dejar clara su intención.

![](assets/using-advanced-smart-list-rule-logic-5.png)

## Utilice paréntesis anidados para cuatro o más filtros si es necesario {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Según su intención, es posible que tenga que agregar paréntesis anidados al utilizar cuatro o más filtros.

![](assets/using-advanced-smart-list-rule-logic-6.png)

>[!TIP]
>
>Si introduce una regla no válida, verá una línea roja debajo de la regla. Desplácese por el texto para ver el mensaje de error relacionado.
