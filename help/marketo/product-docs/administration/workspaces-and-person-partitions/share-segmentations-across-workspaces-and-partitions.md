---
unique-page-id: 7515767
description: Uso compartido de segmentos entre espacios de trabajo y particiones - Documentos de Marketo - Documentación del producto
title: Compartir segmentos entre espacios de trabajo y particiones
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Compartir segmentos entre espacios de trabajo y particiones {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Este artículo es solo para clientes que tienen espacios de trabajo y particiones.

## ¿Qué es una segmentación? {#whats-a-segmentation}

Marketo es bueno en elegir las personas adecuadas para un programa o una campaña inteligente. Sin embargo, para personas más permanentes, debe utilizar las segmentaciones. Son necesarias para utilizar contenido dinámico avanzado en Marketo.

>[!NOTE]
>
>Más información [cómo crear segmentos](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Una vez configurados estos personajes (_y_ si utiliza espacios de trabajo), querrá compartirlos entre sus espacios de trabajo. Estas son algunas cosas buenas que hay que saber:

## Reglas y sugerencias {#rules-tips}

* Cada suscripción a Marketo puede contener hasta 20 segmentos &quot;en total&quot; en varios espacios de trabajo (**no 20 por espacio de trabajo**).
* Solo puede compartir una segmentación con espacios de trabajo a los que tenga acceso.
* Asegúrese de crear y utilizar un **Espacio de trabajo predeterminado que tiene visibilidad en todas las particiones**.

* El procesamiento de la segmentación solo se ejecuta en las personas del espacio de trabajo donde se crea la segmentación.

   * Cree la segmentación que desee compartir dentro del espacio de trabajo predeterminado.
      * Aprobar la segmentación
      * El espacio de trabajo compartido ve una carpeta bloqueada y la segmentación es de solo lectura.
      * La versión compartida no se puede editar. Solo puede editar la Segmentación original en la que se creó.
   * Al hacer clic en un segmento (por ejemplo, el sector sanitario) dentro de una segmentación compartida, las personas que vea solo formarán parte de la partición asociada al espacio de trabajo que esté viendo.
      * Si crea una segmentación en Workspace 1 (WS1) y la comparte con WS2 y WS1 no tiene acceso a la partición para WS2, NO volverá a calcular la segmentación.
      * Si crea una segmentación en un espacio de trabajo que tiene particiones limitadas y luego la comparte con otro espacio de trabajo, ese espacio de trabajo que recibió la segmentación compartida solo verá personas si se superponen.


>[!NOTE]
>
>Algunas de estas reglas son un poco complejas. La forma más sencilla de empezar es realizar pruebas con personas específicas. Siempre puede realizar nuevas segmentaciones y deshacerse de las antiguas.

## Situaciones de ejemplo {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## Uso compartido de una segmentación {#share-a-segmentation}

1. Vaya a la **Base de datos**.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Clic con el botón derecho **Segmentaciones** y seleccione **Nuevas carpetas**.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Asigne un nombre a la carpeta que va a compartir entre espacios de trabajo (por ejemplo: Compartir segmentos).

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Mueva los segmentos que desea compartir a la carpeta .

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Haga clic con el botón derecho en la carpeta y seleccione **Compartir carpeta**.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta. Haga clic en **Guardar**.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >El cuadro de diálogo muestra los espacios de trabajo que tiene permiso para ver, por lo que Marketo recomienda crear y compartir segmentos desde el espacio de trabajo predeterminado que tiene visibilidad en todos los espacios de trabajo y particiones.

La carpeta de origen se muestra en el árbol de bases de datos con una flecha que indica que se comparte con otros espacios de trabajo. Desde el espacio de trabajo compartido, la carpeta se muestra con un bloqueo para indicar que el contenido de la carpeta se ha compartido desde otro espacio de trabajo y que es de solo lectura.
