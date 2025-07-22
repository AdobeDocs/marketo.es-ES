---
unique-page-id: 2359449
description: Definición de reglas de segmentos - Documentos de Marketo - Documentación del producto
title: Definir reglas de segmentos
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
feature: Segmentation
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Definir reglas de segmentos {#define-segment-rules}

La definición de reglas de segmentos le permite clasificar a sus recursos en diferentes grupos mutuamente excluyentes.

>[!PREREQUISITES]
>
>[Crear una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Ir a **[!UICONTROL Base de datos]**.

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Seleccione **[!UICONTROL Segmentaciones]** del árbol y luego haga clic en un **Segmento** en particular.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Haga clic en **[!UICONTROL Lista inteligente]** y agregue filtros.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Los segmentos actualmente no admiten los operadores _En las versiones anteriores_ y _En el intervalo de tiempo_ en los filtros. Esto se debe a que las segmentaciones solo buscan actualizaciones cuando se registra un valor de datos de cambio. Estos valores _no_ se han registrado para cosas que cambian automáticamente, como campos de fórmula y fechas. Además, no se admiten operadores de fecha con intervalos de fecha relativos, ya que se calculan en el momento de la aprobación de la segmentación, no en el momento de una actividad Cambiar valor de datos.

   >[!NOTE]
   >
   >Los filtros &quot;Tipo de SFDC&quot; y &quot;Tipo de Microsoft&quot; actualmente no son compatibles con las listas inteligentes de segmentación.

1. Rellene los valores adecuados para los filtros.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >El comportamiento del registro de actividades para los campos de cuenta puede afectar a la calificación. Por lo tanto, se recomienda evitar el uso de campos de Cuenta al definir reglas de segmento.

1. Haga clic en la ficha **[!UICONTROL Personas (borrador)]** para ver las personas que pueden cumplir los requisitos para ser miembros de este segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Vaya a **[!UICONTROL Acciones de segmentación]**. Haga clic en **[!UICONTROL Aprobar]**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >El número total de segmentos que puede crear en una segmentación depende de la cantidad y el tipo de filtros utilizados, así como de la complejidad de la lógica de los segmentos. Aunque puede crear hasta 100 segmentos utilizando campos estándar, el uso de otros tipos de filtros puede aumentar la complejidad y es posible que la segmentación no se apruebe. Algunos ejemplos son: campos personalizados, miembros de la lista, campos de propietario del posible cliente y fases de ingresos.
   >
   >Si recibe un mensaje de error durante la aprobación y necesita ayuda para reducir la complejidad de la segmentación, comuníquese con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Consulte el panel para obtener una descripción general rápida de los segmentos de un gráfico circular y de las reglas aplicadas.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

¡Buen trabajo! Estos segmentos van a ser útiles en muchos lugares de Marketo.

>[!NOTE]
>
>Una persona podría calificar para diferentes segmentos, pero eventualmente pertenece a solo uno que depende del [orden de prioridad de los segmentos](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>La pantalla [!UICONTROL Personas (Borrador)] muestra todas las personas que cumplen los requisitos para ser miembro y no siempre es la lista final de personas. Apruebe el segmento para ver la lista final.

>[!MORELIKETHIS]
>
>[Aprobar una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
