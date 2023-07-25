---
unique-page-id: 557316
description: 'Definición de filtros de listas inteligentes: Documentos de Marketo, documentación del producto'
title: Definición de filtros de listas inteligentes
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Definición de filtros de listas inteligentes {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](create-a-smart-list.md)
>* [Buscar y agregar filtros a listas inteligentes](find-and-add-filters-to-a-smart-list.md)

Ahora que lo ha hecho [creó una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) y [filtros añadidos](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) para ello, vamos a definir los filtros. Así es como.

Continuando con nuestro ejemplo, definamos estos filtros para encontrar todas las personas en California con una puntuación superior a 50.

1. Ir a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione la lista inteligente y haga clic en **Lista inteligente** pestaña.

   ![](assets/smarlist-choosefilters.png)

1. Buscar y seleccionar **CA** para el **Estado** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Es posible que almacene ambos **California** y **CA**. Para filtrar ambos valores e incluir: _todo_ personas de California, aprendan a  [agregar varios valores a un filtro de lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Elija el **bueno que** operador y escriba **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Si cree que puede tener algunos registros en la base de datos que contienen direcciones de correo electrónico incompletas (por ejemplo, solo &quot;@adobe.com&quot;), utilice **dos** Filtros de direcciones de correo electrónico cuando utiliza el operador &quot;contains&quot;. Un filtro con &quot;contiene @adobe.com&quot; y un filtro independiente con &quot;contiene adobe.com&quot; (excluyendo el símbolo @).

Ahora sabe cómo crear una lista inteligente y añadir o definir filtros.
