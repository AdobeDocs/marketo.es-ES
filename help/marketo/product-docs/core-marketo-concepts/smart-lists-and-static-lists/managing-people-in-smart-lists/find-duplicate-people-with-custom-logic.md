---
unique-page-id: 2952636
description: Encontrar personas duplicadas con lógica personalizada - Documentos de Marketo - Documentación del producto
title: Buscar personas duplicadas con lógica personalizada
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 5%

---

# Buscar personas duplicadas con lógica personalizada {#find-duplicate-people-with-custom-logic}

El Marketo Engage tiene una lista inteligente del sistema que busca personas duplicadas haciendo coincidir sus direcciones de correo electrónico. Si desea utilizar otro campo para buscar duplicados con, así es.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Vaya al área de **[!UICONTROL Actividades de mercadotecnia]**.

![](assets/ma-2.png)

1. Seleccione su lista inteligente y haga clic en la ficha **[!UICONTROL Lista inteligente]**.

   ![](assets/two-4.png)

1. Busque y arrastre el filtro **[!UICONTROL Campos duplicados]** al lienzo.

   ![](assets/three-4.png)

1. Elija una de las cuatro opciones disponibles:

   * Correo electrónico
   * Nombre completo
   * Apellido
   * Actualizado en

   >[!NOTE]
   >
   >Todos los campos, excepto la dirección de correo electrónico, distinguen entre mayúsculas y minúsculas. Por lo tanto, si utiliza &quot;John Doe&quot; en el campo Nombre completo, _no_ devolverá resultados para John Doe.

   ![](assets/four-2.png)

   ¡Listo! Ejecute la lista inteligente para buscar personas con el mismo valor en el campo seleccionado anteriormente.
