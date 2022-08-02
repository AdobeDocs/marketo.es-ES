---
unique-page-id: 557316
description: 'Definir filtros de lista inteligente: documentos de Marketo: documentación del producto'
title: Definir filtros de lista inteligente
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Definir filtros de lista inteligente {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Crear una lista inteligente](create-a-smart-list.md)
>* [Buscar y agregar filtros a listas inteligentes](find-and-add-filters-to-a-smart-list.md)


Ahora que lo ha hecho [crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) y [filtros añadidos](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) a él, vamos a definir los filtros. Así es como.

Siguiendo con nuestro ejemplo, defina estos filtros para encontrar todas las personas en California con una puntuación superior a 50.

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione la lista inteligente y haga clic en el **Lista inteligente** pestaña .

   ![](assets/smarlist-choosefilters.png)

1. Buscar y seleccionar **CA** para el **Estado** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Puede que almacene ambas **California** y **CA**. Para filtrar por ambos valores e incluir _all_ personas de California, aprender a  [agregar varios valores a un filtro de lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Elija el **bueno que** operador e introduzca **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Si cree que puede tener algunos registros en la base de datos que contengan direcciones de correo electrónico incompletas (por ejemplo, solo &quot;@adobe.com&quot;), utilice **two** Filtros de dirección de correo electrónico cuando utiliza el operador &quot;contiene&quot;. Un filtro con &quot;contiene @adobe.com&quot; y otro con &quot;contiene adobe.com&quot; (sin incluir el símbolo @).

Ahora sabe cómo crear una lista inteligente y añadir/definir filtros.
