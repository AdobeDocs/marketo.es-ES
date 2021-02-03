---
unique-page-id: 37355758
description: Añadir miembros a un Programa de Evento - Documentos de marketing - Documentación del producto
title: Añadir miembros a un Programa de Evento
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Añadir miembros a un Programa de Evento {#adding-members-to-an-event-program}

Este artículo solo se aplica a los usuarios que utilizan los Objetivos de Evento o Límite de Eventos.

>[!CAUTION]
>
>La importación de una lista de personas directamente en un Programa de Evento impedirá que esos registros se cuenten en los registros reales en el informe Seguimiento de objetivos y en el informe Progresión de límite de Eventos. Siga las instrucciones que se indican a continuación para asegurarse de que se cuentan sus registros.

1. Cree y [agregue personas a una lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Cree una campaña](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) inteligente.

1. En la Lista inteligente de la Campaña inteligente que creó en el paso dos, busque y agregue el filtro **Miembro de Lista**.

   ![](assets/three.png)

1. Busque y seleccione la lista que creó en el paso uno.

   ![](assets/four.png)

1. En Flujo, busque y agregue el paso de flujo **Cambiar estado de Programa**.

   ![](assets/five.png)

1. Busque y seleccione su Programa de Evento.

   ![](assets/six.png)

1. Elija el estado que desee.

   ![](assets/seven.png)

1. En la ficha Programación, haga clic en **Ejecutar una vez**.

   ![](assets/eight.png)

1. Seleccione **Ejecutar ahora** y haga clic en **Ejecutar**.

   ![](assets/nine.png)

1. Una vez ejecutada la campaña inteligente, los miembros se agregan al programa y se contarán en los cálculos de Seguimiento de objetivos y Progreso de límite de Evento.
