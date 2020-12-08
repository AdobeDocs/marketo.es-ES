---
unique-page-id: 7515767
description: Compartir segmentos entre espacios de trabajo y particiones - Documentos de marketing - Documentación del producto
title: Compartir segmentos entre espacios de trabajo y particiones
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---


# Compartir segmentos entre espacios de trabajo y particiones {#share-segmentations-across-workspaces-and-partitions}

>[!NOTE]
>
>**Requisitos previos**
>
>Este artículo es solo para clientes que tienen espacios de trabajo y particiones

## ¿Qué es una segmentación? {#whats-a-segmentation}

Marketo es bueno en elegir sólo a las personas adecuadas para un programa o una campaña inteligente. Sin embargo, para personas más permanentes, debe utilizar las segmentaciones. Se necesitan para utilizar contenido dinámico avanzado en Marketing Cloud.

>[!NOTE]
>
>**Buceo profundo**
>
>Aprenda [a crear segmentaciones](../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Una vez configuradas estas personas (**y que** utilice espacios de trabajo), querrá compartirlas entre los espacios de trabajo. A continuación se presentan algunas cosas buenas que saber:

## Reglas y sugerencias {#rules-tips}

* Cada suscripción de marketing puede contener hasta 20 segmentos &quot;en total&quot; en varias áreas de trabajo (**no 20 por espacio de trabajo**).
* Solo puede compartir una segmentación con espacios de trabajo a los que tenga acceso.
* Asegúrese de crear y utilizar un espacio de trabajo **Predeterminado que tenga visibilidad en todas las particiones**.

* El procesamiento de la segmentación solo se ejecuta en las personas del espacio de trabajo donde se crea la segmentación.

   * Cree la segmentación que desee compartir dentro del espacio de trabajo predeterminado.

      * Aprobar la segmentación
      * El espacio de trabajo compartido ve una carpeta bloqueada y la segmentación es de solo lectura.
      * No se puede editar la versión compartida. Solo puede editar la segmentación original donde se creó.
   * Al hacer clic en un segmento (por ejemplo, de salud) dentro de una segmentación compartida, las personas que vea serán sólo las personas en la partición asociadas con el espacio de trabajo que esté viendo.

      * Si crea una segmentación en Workspace 1 (WS1) y la comparte con WS2 y WS1 no tiene acceso a la partición para WS2, NO volverá a calcular la segmentación.
      * Si crea una segmentación en un espacio de trabajo que tiene particiones limitadas y luego la comparte con otro espacio de trabajo, ese espacio de trabajo que recibió la segmentación compartida solo verá a las personas si se superponen.


>[!NOTE]
>
>Algunas de estas reglas son un poco complejas. La manera más fácil de empezar es probarla con personas específicas. Siempre puede crear nuevas segmentaciones y deshacerse de las antiguas.

## Escenarios de ejemplo {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

** ![](assets/image2015-5-27-16-3a26-3a48.png)

**

## Compartir una segmentación {#share-a-segmentation}

1. Vaya a la base de datos.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Haga clic con el botón derecho en Segmentos y seleccione Nuevas carpetas.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Asigne un nombre a la carpeta que va a compartir entre espacios de trabajo (ejemplo: Compartir segmentos).

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Mueva los segmentos que desee compartir a la carpeta.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Haga clic con el botón derecho en la carpeta y seleccione Compartir carpeta.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta. Haga clic en Guardar.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >El cuadro de diálogo muestra los espacios de trabajo con los que tiene permiso para vista, por lo que Marketing recomienda crear y compartir segmentos desde el espacio de trabajo Predeterminado que tiene visibilidad en todos los espacios de trabajo y particiones.

La carpeta de origen se muestra en el árbol Base de datos con una flecha que indica que se comparte con otros espacios de trabajo. Desde el espacio de trabajo compartido, la carpeta se muestra con un bloqueo para indicar que el contenido de la carpeta se ha compartido desde otro espacio de trabajo y es de sólo lectura.

>[!NOTE]
>
>**Artículos relacionados**
>
>[Segmentación y recortes](http://docs.marketo.com/display/docs/segmentation+and+snippets)

