---
unique-page-id: 2359449
description: Definición de reglas de segmentos - Documentos de Marketo - Documentación del producto
title: Definir reglas de segmentos
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Definir reglas de segmentos {#define-segment-rules}

La definición de reglas de segmentos le permite clasificar a sus recursos en diferentes grupos mutuamente excluyentes.

>[!PREREQUISITES]
>
>[Creación de una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Vaya a la **Base de datos.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Seleccionar **Segmentación** en el árbol y, a continuación, haga clic en una **Segmento**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Clic **Lista inteligente** y agregue filtros.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Los segmentos no son compatibles actualmente _En el pasado_ y _En intervalo de tiempo_  operadores en filtros. Esto se debe a que las segmentaciones solo buscan actualizaciones cuando se registra un valor de datos de cambio. Estos valores son _no_ registrado para cosas que cambian automáticamente, como campos de fórmula y fechas. Además, no se admiten operadores de fecha con intervalos de fecha relativos, ya que se calculan en el momento de la aprobación de la segmentación, no en el momento de una actividad Cambiar valor de datos.

   >[!NOTE]
   >
   >Los filtros &quot;Tipo SFDC&quot; y &quot;Tipo Microsoft&quot; actualmente no son compatibles con las listas inteligentes de segmentación.

1. Rellene los valores adecuados para los filtros.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >El comportamiento del registro de actividades para los campos de cuenta puede afectar a la calificación. Por lo tanto, se recomienda evitar el uso de campos de Cuenta al definir reglas de segmento.

1. Haga clic en **Personas (borrador)** para ver las personas que pueden cumplir los requisitos para ser miembros de este segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Ir a **Acciones de segmentación**. Clic **Aprobar**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >El número total de segmentos que puede crear en una segmentación depende de la cantidad y el tipo de filtros utilizados, así como de la complejidad de la lógica de los segmentos. Aunque puede crear hasta 100 segmentos utilizando campos estándar, el uso de otros tipos de filtros puede aumentar la complejidad y es posible que la segmentación no se apruebe. Algunos ejemplos son: campos personalizados, miembros de la lista, campos de propietario del posible cliente y fases de ingresos.
   >
   >Si recibe un mensaje de error durante la aprobación y necesita ayuda para reducir la complejidad de la segmentación, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Consulte el panel para obtener una descripción general rápida de los segmentos de un gráfico circular y de las reglas aplicadas.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

¡Buen trabajo! Estos segmentos van a ser útiles en muchos lugares de Marketo.

>[!NOTE]
>
>Una persona puede cumplir los requisitos para diferentes segmentos, pero finalmente pertenece a solo uno que depende de la variable [orden de prioridad de los segmentos](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>La pantalla Personas (Borrador) muestra todas las personas que cumplen los requisitos para ser miembros y no siempre es la lista final de personas. Apruebe el segmento para ver la lista final.

>[!MORELIKETHIS]
>
>[Aprobación de una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
