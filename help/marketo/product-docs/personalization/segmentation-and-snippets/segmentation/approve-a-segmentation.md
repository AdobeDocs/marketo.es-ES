---
unique-page-id: 2359457
description: Aprenda a aprobar una segmentación para que se pueda utilizar en el contenido dinámico y la creación de informes. Utilice las acciones de base de datos y segmentación para aprobar después de definir las reglas de segmentos.
title: Aprobar una segmentación
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
TQID: https://experienceleague.adobe.com/hvFKybwLh1INYx2YWtOmdebJVYXOzhNMMncqeOoV8EU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 5%

---

# Aprobar una segmentación {#approve-a-segmentation}

Es necesario aprobar una segmentación para poder utilizarla.

>[!PREREQUISITES]
>
>* [Crear una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Definir reglas de segmentos](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Se puede aprobar un máximo de 20 segmentos a la vez.

1. Ir a **[!UICONTROL Base de datos]**.

   ![](assets/approve-a-segmentation-1.png)

1. En la segmentación, haga clic en **[!UICONTROL Acciones de segmentación]** y, a continuación, en **[!UICONTROL Aprobar]**.

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >El estado cambia a _Aprobando_ mientras la aprobación está en proceso.

   >[!CAUTION]
   >
   >La aprobación puede tardar entre unos minutos y un día o dos en completarse, según el tamaño de la base de datos.

1. Una vez aprobado, el [!UICONTROL estado] cambia de [!UICONTROL Aprobando] a [!UICONTROL Aprobado].

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >El número de personas de cada segmento se muestra entre corchetes junto al nombre del segmento.

1. La ficha **[!UICONTROL Personas]** del **[!UICONTROL Segmento]** muestra ahora la lista final de personas para el segmento.

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>El número total de segmentos que puede crear en una segmentación depende de la cantidad y el tipo de filtros utilizados, así como de la complejidad de la lógica de los segmentos. Aunque puede crear hasta 100 segmentos utilizando campos estándar, el uso de otros tipos de filtros puede aumentar la complejidad y es posible que la segmentación no se apruebe. Algunos ejemplos son: campos personalizados, miembros de la lista, campos de propietario del posible cliente y fases de ingresos.
>
>Si recibe un mensaje de error durante la aprobación y necesita ayuda para reducir la complejidad de la segmentación, comuníquese con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Usar filtros de segmento en una lista inteligente](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
