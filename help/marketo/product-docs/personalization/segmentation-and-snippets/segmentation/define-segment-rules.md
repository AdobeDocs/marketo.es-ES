---
unique-page-id: 2359449
description: Definir reglas de segmentos - Documentos de marketing - Documentación del producto
title: Definir reglas de segmentos
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---


# Definir reglas de segmentos {#define-segment-rules}

La definición de reglas de segmentos le permite categorizar a sus personas en diferentes grupos mutuamente excluyentes.

>[!PREREQUISITES]
>
>[Crear una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Vaya a la **base de datos.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Haga clic en la **Segmentación** del árbol y, a continuación, haga clic en un segmento **concreto**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Haga clic en **Lista inteligente** y agregue filtros.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Actualmente, los segmentos no admiten los operadores _En filtros anteriores_ y _En intervalo de tiempo_. Esto se debe a que las segmentaciones solo buscan actualizaciones cuando se registra un valor de datos de cambio. Estos valores se registran _no_ para cosas que cambian automáticamente, como campos de fórmula y fechas. Además, los operadores de fecha con intervalos de fechas relativos no son compatibles, ya que se calculan en el momento de la aprobación de la segmentación, no en el momento de una actividad Cambiar valor de datos.

   >[!NOTE]
   >
   >Las filtros &quot;Tipo de SFDC&quot; y &quot;Tipo de Microsoft&quot; no son compatibles actualmente con las listas inteligentes de segmentación.

1. Rellene los valores adecuados para los filtros.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >Las Listas inteligentes son increíbles. [Más información sobre ellos](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md).

1. Haga clic en la ficha **Personas (borrador)** para vista de las personas que pueden calificar para ser miembros de este segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Vaya a **Acciones de segmentación**. Haga clic en **Aprobar**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >El número total de segmentos que puede crear en una segmentación depende del número y el tipo de filtros utilizados y también de la complejidad de la lógica de los segmentos. Aunque puede crear hasta 100 segmentos mediante campos estándar, el uso de otros tipos de filtros puede aumentar la complejidad y la segmentación podría no aprobarse. Algunos ejemplos son: campos personalizados, miembro de lista, campos de propietario de posibles clientes y etapas de ingresos.
   >
   >Si recibe un mensaje de error durante la aprobación y necesita ayuda para reducir la complejidad de la segmentación, póngase en contacto con [Soporte técnico de marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Consulte el panel para obtener una descripción general rápida de los segmentos en un gráfico circular, así como las reglas aplicadas.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

¡Buen trabajo! Estos segmentos serán útiles en muchos lugares de Marketing.

>[!NOTE]
>
>Una persona puede cumplir los requisitos para distintos segmentos, pero finalmente pertenece a uno solo que depende del [orden de prioridad de los segmentos](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>La pantalla Personas (Borrador) muestra todas las personas que califican para ser miembros y no siempre es la lista final de las personas. Apruebe el segmento para ver la lista final.

>[!MORELIKETHIS]
>
>[Aprobar una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
