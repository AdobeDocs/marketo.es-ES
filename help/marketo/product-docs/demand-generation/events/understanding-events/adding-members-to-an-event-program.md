---
unique-page-id: 37355758
description: 'Adición de miembros a un programa de eventos: Marketo Docs: documentación del producto'
title: Adición de miembros a un programa de eventos
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Adición de miembros a un programa de eventos {#adding-members-to-an-event-program}

Este artículo solo se aplica a los usuarios que utilizan el límite de eventos o los objetivos de evento.

>[!CAUTION]
>
>La importación de una lista de personas directamente en un programa de eventos impedirá que esos registros se cuenten en registros reales en el informe de seguimiento de objetivos y en el informe de progresión de límite de eventos . Siga las instrucciones que se indican a continuación para asegurarse de que sus registros se cuentan.

1. Crear y [agregar personas a una lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Creación de una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. En la lista inteligente de la campaña inteligente que ha creado en el paso 2, busque y añada la variable **Miembro de la lista** filtro.

   ![](assets/three.png)

1. Busque y seleccione la lista que creó en el paso uno.

   ![](assets/four.png)

1. En Flujo, busque y añada la variable **Cambiar estado del programa** paso de flujo.

   ![](assets/five.png)

1. Busque y seleccione el Programa de eventos.

   ![](assets/six.png)

1. Elija el estado que desee.

   ![](assets/seven.png)

1. En la ficha Programación, haga clic en **Ejecutar una vez**.

   ![](assets/eight.png)

1. Select **Ejecutar ahora** y haga clic en **Ejecutar**.

   ![](assets/nine.png)

1. Una vez ejecutada la campaña inteligente, los miembros se añaden al programa y se cuentan en los cálculos de Seguimiento de objetivos y Progreso de límite de eventos .
