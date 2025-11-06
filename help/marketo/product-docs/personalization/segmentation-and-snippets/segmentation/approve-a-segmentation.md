---
unique-page-id: 2359457
description: 'Aprobación de una segmentación: documentos de Marketo, documentación del producto'
title: Aprobar una segmentación
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: b29186ba84ec88be42432e56d1ad0e77c5b43900
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 2%

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
