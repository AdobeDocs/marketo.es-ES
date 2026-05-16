---
unique-page-id: 2952636
description: Aprenda a encontrar personas duplicadas con lógica personalizada. Cree una lista inteligente para identificar duplicados según sus criterios.
title: Buscar personas duplicadas con lógica personalizada
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
TQID: https://experienceleague.adobe.com/-NvWt-eEzngL0QY7Kyl6lfjd75WcoQmcq3IiN7Uc6-w
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 12%

---

# Buscar personas duplicadas con lógica personalizada {#find-duplicate-people-with-custom-logic}

Marketo Engage tiene una lista inteligente del sistema que busca personas duplicadas haciendo coincidir sus direcciones de correo electrónico. Si desea utilizar otro campo para buscar duplicados con, siga los pasos a continuación.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Vaya al área **[!UICONTROL Actividades de marketing]**.

![](assets/ma-2.png)

1. Seleccione su lista inteligente y haga clic en la ficha **[!UICONTROL Lista inteligente]**.

   ![](assets/two-4.png)

1. Busque y arrastre el filtro **[!UICONTROL Campos duplicados]** al lienzo.

   ![](assets/three-4.png)

1. Elija una de las cuatro opciones disponibles:

   * [!UICONTROL Dirección de correo electrónico]
   * [!UICONTROL Nombre completo]
   * [!UICONTROL Apellidos]
   * [!UICONTROL Actualizado A Las]

   >[!NOTE]
   >
   >Todos los campos, excepto la dirección de correo electrónico, distinguen entre mayúsculas y minúsculas. Por lo tanto, si utiliza &quot;John Doe&quot; en el campo Nombre completo, _no_ devolverá resultados para John Doe.

   ![](assets/four-2.png)

   Ejecute la lista inteligente para buscar personas con el mismo valor en el campo seleccionado anteriormente.
