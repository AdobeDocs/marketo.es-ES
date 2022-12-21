---
unique-page-id: 2952636
description: Buscar personas duplicadas con lógica personalizada - Documentos de Marketo - Documentación del producto
title: Buscar personas duplicadas con lógica personalizada
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 6%

---

# Buscar personas duplicadas con lógica personalizada {#find-duplicate-people-with-custom-logic}

Marketo tiene una lista inteligente del sistema que encuentra personas duplicadas al hacer coincidir sus direcciones de correo electrónico. Si desea utilizar otro campo con el que buscar duplicados, así es como.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Vaya a la **Actividades de marketing** .

![](assets/ma-2.png)

1. Seleccione la lista inteligente y haga clic en el **Lista inteligente** pestaña .

   ![](assets/two-4.png)

1. Busque y arrastre el **Duplicar campos** filtre al lienzo.

   ![](assets/three-4.png)

1. Elija una de las cuatro opciones disponibles:

   * Dirección de email
   * Nombre completo
   * Apellido
   * Actualizado en

   >[!NOTE]
   >
   >Todos los campos, con la excepción de Dirección de correo electrónico, distinguen entre mayúsculas y minúsculas. Así que usar &quot;john doe&quot; en el campo Nombre completo _not_ devuelve resultados para John Doe.

   ![](assets/four-2.png)

   Listo! Ejecute la lista inteligente para buscar personas con el mismo valor en el campo seleccionado anteriormente.
