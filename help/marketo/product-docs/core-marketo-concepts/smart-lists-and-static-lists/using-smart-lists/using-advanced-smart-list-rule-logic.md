---
unique-page-id: 1146901
description: Uso de la lógica avanzada de reglas de Lista inteligente - Documentos de marketing - Documentación del producto
title: Uso de la lógica avanzada de reglas de Lista inteligente
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Uso de la lógica avanzada de reglas de Lista inteligente {#using-advanced-smart-list-rule-logic}

Puede encontrar las personas exactas que necesita aplicando la lógica de regla de lista inteligente a varios filtros dentro de una lista inteligente. Así es como.

>[!PREREQUISITES]
>
>* [Buscar y Añadir Filtros en una Lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definir Filtros de Lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>



>[!NOTE]
>
>La lógica de filtro avanzada solo está disponible si hay tres o más filtros en la lista inteligente.

## Añadir la lógica en una Lista inteligente {#add-logic-to-a-smart-list}

De forma predeterminada, su lista inteligente encontrará las personas que coinciden con los filtros **ALL** (filtros 1 *y* 2 *y* 3). Puede cambiar la lógica de la regla para buscar personas que coincidan con **CUALQUIER** de los filtros definidos (filtros 1 *o* 2 *o* 3), o utilizar filtros avanzados (filtros 1 *y* 2 *o *3).

En este ejemplo, supongamos que desea encontrar personas en California *y* con una puntuación de al menos 50 puntos *o* con un estado de &quot;Ventas calificadas&quot;.

1. Seleccione **Usar** **Avanzadas** **filtros** en la lista desplegable.

   ![](assets/one.png)

   >[!NOTE]
   >
   >El uso de filtros **Advanced** reduce la necesidad de crear listas inteligentes con el miembro del filtro de Lista inteligente. Esto ayuda a optimizar el rendimiento.

1. El cuadro de texto **filtros** **avanzados** mostrará &quot;y&quot; como el valor predeterminado entre todos sus filtros.

   ![](assets/two-2.png)

1. Escriba un par de paréntesis alrededor de &quot;2 y 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Debe utilizar &quot;y&quot; antes de &quot;o&quot; al introducir la lógica de regla.

1. Cambie &quot;y&quot; entre &quot;2 y 3&quot; por &quot;o&quot;.

   ![](assets/four-1.png)

## Usar paréntesis al mezclar &quot;And&quot; y &quot;Or {#use-parentheses-when-mixing-and-and-or}

La combinación de la lógica &quot;y&quot; y &quot;o&quot; requiere paréntesis para dejar clara su intención.

![](assets/advancedfilters-parent.png)

## Utilice paréntesis anidados para cuatro o más Filtros si es necesario {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Según su intención, es posible que necesite agregar paréntesis anidados al usar cuatro o más filtros.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Si introduce una regla no válida, verá una línea roja debajo de la regla. Desplácese por el texto para ver el mensaje de error relacionado.

