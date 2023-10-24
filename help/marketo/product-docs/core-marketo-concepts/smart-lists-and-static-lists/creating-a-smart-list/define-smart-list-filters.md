---
unique-page-id: 557316
description: 'Definición de filtros de listas inteligentes: Documentos de Marketo, documentación del producto'
title: Definición de filtros de listas inteligentes
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Definición de filtros de listas inteligentes {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Buscar y agregar filtros a listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Ahora que lo ha hecho [creó una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} and [added filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} para ello, vamos a definir los filtros. Así es como.

Continuando con nuestro ejemplo, definamos estos filtros para encontrar todas las personas en California con una puntuación superior a 50.

1. Ir a **[!UICONTROL Actividades de marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione la lista inteligente y haga clic en **[!UICONTROL Lista inteligente]** pestaña.

   ![](assets/smarlist-choosefilters.png)

1. Busque y seleccione &quot;CA&quot; para **[!UICONTROL Estado]** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Es posible que almacene tanto &quot;California&quot; como &quot;CA&quot;. Para filtrar ambos valores e incluir: _todo_ personas de California, aprendan a  [agregar varios valores a un filtro de listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Elija el **[!UICONTROL mayor que]** y escriba &quot;50&quot;.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Si cree que puede tener algunos registros en la base de datos que contienen direcciones de correo electrónico incompletas (por ejemplo, &quot;@adobe.com&quot;), utilice dos filtros de dirección de correo electrónico cuando utilice el operador &quot;contains&quot;. Un filtro con &quot;contiene @adobe.com&quot; y un filtro independiente con &quot;contiene adobe.com&quot; (excluyendo el símbolo @).

Ahora sabe cómo crear una lista inteligente y agregar o definir filtros.
