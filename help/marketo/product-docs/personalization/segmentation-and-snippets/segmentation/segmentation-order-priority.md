---
unique-page-id: 2359500
description: Obtenga información acerca de la prioridad de orden de segmentación y cómo determina a qué segmento pertenece una persona. Edite el orden de los segmentos en la base de datos para controlar la evaluación de los segmentos.
title: Prioridad de orden de segmentación
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
TQID: https://experienceleague.adobe.com/wDvufJzxu0BFCSov4etUpEMxaol3-R5CePqllYyDeSc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 144
ht-degree: 4%

---

# Prioridad de orden de segmentación {#segmentation-order-priority}

Es importante comprender cómo **order** establece la prioridad para la evaluación de sus recursos en una segmentación.

>[!PREREQUISITES]
>
>[Crear una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[Definir reglas de segmentos ](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Solo puede editar una segmentación en modo de borrador.

1. Ir a **Base de datos**.

   ![](assets/segmentation-order-priority-1.png)

1. Seleccione su **segmentación**. En **[!UICONTROL Acciones de segmentación]**, haga clic en **[!UICONTROL Editar segmentos]**.

   ![](assets/segmentation-order-priority-2.png)

   Puede comprobar o editar el orden de los segmentos desde esta pantalla.

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* Los segmentos son mutuamente excluyentes. Una persona solo puede ser miembro de un segmento a la vez.
>* Cuando una persona cumple los requisitos para dos segmentos, solo pertenece al primero de la lista.
>* Si una persona no cumple los requisitos para ningún segmento, se convertirá en miembro del segmento predeterminado.
