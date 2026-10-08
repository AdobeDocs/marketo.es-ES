---
unique-page-id: 557316
description: Obtenga información sobre cómo definir filtros de listas inteligentes. Establezca restricciones y valores de filtro para determinar quién aparece en la lista.
title: Definir filtros de la lista inteligente
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/gCJT14FtnJaPAMhDUWI7XpoST1lc9yvzZbVKq-oTx-w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 6%
---
# Definir filtros de la lista inteligente {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Buscar y agregar filtros a listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Ahora que ha [creado una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} y [agregado filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} a ella, defina los filtros de la siguiente manera.

Siguiendo con este ejemplo, defina estos filtros para buscar todas las personas en California con una puntuación superior a 50.

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
>Si cree que puede tener algunos registros en la base de datos que contienen direcciones de correo electrónico incompletas (por ejemplo, solo &quot;@adobe.com&quot;), utilice dos filtros de dirección de correo electrónico cuando utilice el operador &quot;contains&quot;. Un filtro con &quot;contiene @adobe.com&quot; y un filtro independiente con &quot;contiene adobe.com&quot; (excluyendo el símbolo @).

Ahora sabe cómo crear una lista inteligente y agregar o definir filtros.
