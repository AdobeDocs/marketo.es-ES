---
unique-page-id: 37355758
description: Adición de miembros a un programa de eventos - Documentos de Marketo - Documentación del producto
title: Adición de miembros a un programa de eventos
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 6%

---

# Adición de miembros a un programa de eventos {#adding-members-to-an-event-program}

Este artículo solo se aplica a los usuarios que utilizan el Límite de eventos o los Objetivos de eventos.

>[!CAUTION]
>
>La importación de una lista de personas directamente en un programa de eventos evitará que esos registros se cuenten en registros reales en los informes Seguimiento de objetivos y Progresión del límite de eventos. Siga las instrucciones que se indican a continuación para asegurarse de que se cuentan sus registros.

1. Crear y [agregar personas a una lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Crear una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. En la lista inteligente de la campaña inteligente que creó en el paso 2, busque y agregue el filtro **[!UICONTROL Miembro de la lista]**.

   ![](assets/three.png)

1. Busque y seleccione la lista que creó en el paso uno.

   ![](assets/four.png)

1. En el flujo, busque y agregue el paso de flujo **[!UICONTROL Cambiar estado del programa]**.

   ![](assets/five.png)

1. Busque y seleccione su programa de eventos.

   ![](assets/six.png)

1. Elija el estado que desee.

   ![](assets/seven.png)

1. En la ficha [!UICONTROL Programar], haga clic en **[!UICONTROL Ejecutar una vez]**.

   ![](assets/eight.png)

1. Seleccione **[!UICONTROL Ejecutar ahora]** y haga clic en **[!UICONTROL Ejecutar]**.

   ![](assets/nine.png)

1. Después de que se ejecute la campaña inteligente, los miembros se agregan al programa y contarán en los cálculos Seguimiento de objetivos y Progresión del límite de eventos.
