---
unique-page-id: 2359449
description: Definir reglas de segmentos - Documentos de marketing - Documentación del producto
title: Definir reglas de segmentos
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# Definir reglas de segmentos {#define-segment-rules}

La definición de reglas de segmentos le permite categorizar a sus personas en diferentes grupos mutuamente excluyentes.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!PREREQUISITES]
>
>[Crear una segmentación](create-a-segmentation.md)

1. Vaya a la **base de datos.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Haga clic en **Segmentación **desde el árbol y, a continuación, haga clic en un **segmento** concreto.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Haga clic en Lista **** inteligente y agregue filtros.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Actualmente, los segmentos no admiten *los operadores Anterior* y *Intervalo de tiempo de *en filtros. Esto se debe a que las segmentaciones solo buscan actualizaciones cuando se registra un valor de datos de cambio. Estos valores *no se registran* para los elementos que cambian automáticamente, como los campos de fórmula y las fechas. Además, los operadores de fecha con intervalos de fechas relativos no son compatibles, ya que se calculan en el momento de la aprobación de la segmentación, no en el momento de una actividad Cambiar valor de datos.

   >[!NOTE]
   >
   >Las filtros &quot;Tipo de SFDC&quot; y &quot;Tipo de Microsoft&quot; no son compatibles actualmente con las listas inteligentes de segmentación.

1. Rellene los valores adecuados para los filtros.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >**Buceo profundo**
   >
   >
   >Las Listas inteligentes son increíbles. Aprenda todo lo que puede hacer con Listas [inteligentes y Listas](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)estáticas.

1. Haga clic en la ficha **Personas (borrador)** para vista de las personas que pueden cumplir los requisitos para ser miembros de este segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Vaya a Acciones **de segmentación**. Haga clic en **Aprobar**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >El número total de segmentos que puede crear en una segmentación depende del número y el tipo de filtros utilizados y también de la complejidad de la lógica de los segmentos. Aunque puede crear hasta 100 segmentos mediante campos estándar, el uso de otros tipos de filtros puede aumentar la complejidad y la segmentación podría no aprobarse. Algunos ejemplos son: campos personalizados, miembro de lista, campos de propietario de posibles clientes y etapas de ingresos.
   >
   >
   >Si recibe un mensaje de error durante la aprobación y necesita ayuda para reducir la complejidad de la segmentación, póngase en contacto con la asistencia técnica [de marketing](http://nation.marketo.com/t5/Support/ct-p/Support).

1. Consulte el panel para obtener una descripción general rápida de los segmentos en un gráfico circular, así como las reglas aplicadas.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

¡Buen trabajo! Estos segmentos serán útiles en muchos lugares de Marketing.

>[!NOTE]
>
>Una persona puede calificar para diferentes segmentos, pero finalmente pertenece a uno solo que depende del orden de [prioridad de los segmentos](segmentation-order-priority.md).

>[!NOTE]
>
>**Recordatorio**
>
>La pantalla Personas (Borrador) muestra todas las personas que califican para ser miembros y no siempre es la lista final de las personas. Apruebe el segmento para ver la lista final.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Aprobar una segmentación](approve-a-segmentation.md)

>



