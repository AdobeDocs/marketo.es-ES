---
unique-page-id: 2952636
description: Buscar personas duplicadas con lógica personalizada - Marketo Docs - Documentación del producto
title: Buscar personas duplicadas con lógica personalizada
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Buscar personas duplicadas con lógica personalizada {#find-duplicate-people-with-custom-logic}

Marketo tiene una lista inteligente del sistema que encuentra personas duplicadas al hacer coincidir sus direcciones de correo electrónico. Si desea utilizar otro campo con el que buscar duplicados, así es como.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Vaya al área **Marketing Activities** .

![](assets/ma-2.png)

1. Seleccione la lista inteligente, haga clic en la pestaña **Smart List**.

   ![](assets/two-4.png)

1. Busque y arrastre el filtro **Duplicate Fields** al lienzo.

   ![](assets/three-4.png)

1. Elija una de las cuatro opciones disponibles:

   * Dirección de correo electrónico
   * Nombre completo
   * Apellidos
   * Actualizado en

   >[!NOTE]
   >
   >Todos los campos, con la excepción de Dirección de correo electrónico, distinguen entre mayúsculas y minúsculas. Por lo tanto, el uso de &quot;john doe&quot; en el campo Nombre completo _no_ devolverá resultados para John Doe.

   ![](assets/four-2.png)

   ¡Listo! Ejecute la lista inteligente para buscar personas con el mismo valor en el campo seleccionado anteriormente.
