---
unique-page-id: 557316
description: 'Definición de filtros de listas inteligentes: Documentos de Marketo, documentación del producto'
title: Definición de filtros de listas inteligentes
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Definición de filtros de listas inteligentes {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Buscar y agregar filtros a listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Ahora que ha [creado una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} y [agregado filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} a ella, vamos a definir los filtros. Así es como.

Continuando con nuestro ejemplo, definamos estos filtros para encontrar todas las personas en California con una puntuación superior a 50.

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/define-smart-list-filters-1.png)

1. Seleccione la lista inteligente que desee y haga clic en la ficha **[!UICONTROL Lista inteligente]**.

   ![](assets/define-smart-list-filters-2.png)

1. Busque y seleccione &quot;CA&quot; para el filtro **[!UICONTROL Estado]**.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Es posible que almacene tanto &quot;California&quot; como &quot;CA&quot;. Para filtrar ambos valores e incluir _todas_ las personas de California, aprenda a [agregar varios valores a un filtro de listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Elija el operador **[!UICONTROL greater than]** y escriba &quot;50&quot;.

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Si cree que puede tener algunos registros en la base de datos que contienen direcciones de correo electrónico incompletas (por ejemplo, &quot;@adobe.com&quot;), utilice dos filtros de dirección de correo electrónico cuando utilice el operador &quot;contains&quot;. Un filtro con &quot;contiene @adobe.com&quot; y un filtro independiente con &quot;contiene adobe.com&quot; (excluyendo el símbolo @).

Ahora sabe cómo crear una lista inteligente y agregar o definir filtros.
