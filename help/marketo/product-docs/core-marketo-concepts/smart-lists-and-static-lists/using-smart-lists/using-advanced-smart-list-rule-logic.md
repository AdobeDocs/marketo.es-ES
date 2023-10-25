---
unique-page-id: 1146901
description: Uso de la lógica de regla de listas inteligentes avanzada - Documentos de Marketo - Documentación del producto
title: Uso de la lógica de regla de listas inteligentes avanzadas
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: 8a5903fa5313e34f448f833f20ab8e3624cf23e6
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Uso de la lógica de regla de listas inteligentes avanzadas {#using-advanced-smart-list-rule-logic}

Puede encontrar exactamente las personas que necesita aplicando la lógica de regla de listas inteligentes a varios filtros dentro de una lista inteligente. Así es como.

>[!PREREQUISITES]
>
>* [Buscar y agregar filtros a una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}
>* [Definición de filtros de listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md){target="_blank"}

>[!NOTE]
>
>La lógica de filtro avanzada solo está disponible si hay tres o más filtros en la lista inteligente.

## Agregar lógica a una lista inteligente {#add-logic-to-a-smart-list}

De forma predeterminada, la lista inteligente encontrará las personas que coinciden con **[!UICONTROL TODO]** filtros (filtros 1) _y_ 2 _y_ 3). Puede cambiar la lógica de la regla para buscar personas que coincidan **[!UICONTROL CUALQUIERA]** de los filtros definidos (filtros 1) _o_ 2 _o_ 3) o utilice filtros avanzados (filtros 1) _y_ 2 _o_ 3).

En este ejemplo, supongamos que desea buscar personas en California _y_ con una puntuación de al menos 50 puntos _o_ con el estado &quot;Ventas cualificadas&quot;.

1. Seleccionar **[!UICONTROL Uso de filtros avanzados]** de la lista desplegable.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Uso de **[!UICONTROL Avanzadas]** Los filtros reducen la necesidad de crear listas inteligentes con el filtro Miembro de listas inteligentes. Esto ayuda a optimizar el rendimiento.

1. El **[!UICONTROL Filtros avanzados]** El cuadro de texto mostrará &quot;y&quot; como valor predeterminado entre todos los filtros.

   ![](assets/two-2.png)

1. Escriba un par de paréntesis alrededor de &quot;2 y 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Debe utilizar &quot;y&quot; antes de &quot;o&quot; al introducir la lógica de regla.

1. Cambie &quot;and&quot; entre &quot;2 y 3&quot; y &quot;or&quot;.

   ![](assets/four-1.png)

## Utilice Paréntesis Al Combinar &quot;And&quot; Y &quot;Or {#use-parentheses-when-mixing-and-and-or}

La combinación de las lógicas &quot;and&quot; y &quot;or&quot; requiere paréntesis para dejar clara su intención.

![](assets/advancedfilters-parent.png)

## Utilice paréntesis anidados para cuatro o más filtros si es necesario {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Según su intención, es posible que tenga que agregar paréntesis anidados al utilizar cuatro o más filtros.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Si introduce una regla no válida, verá una línea roja debajo de la regla. Desplácese por el texto para ver el mensaje de error relacionado.
