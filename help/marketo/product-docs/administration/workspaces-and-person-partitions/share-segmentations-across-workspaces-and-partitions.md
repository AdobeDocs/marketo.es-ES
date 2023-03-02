---
unique-page-id: 7515767
description: Uso compartido de segmentaciones en espacios de trabajo y particiones - Documentos de Marketo - Documentación del producto
title: Uso compartido de segmentaciones en espacios de trabajo y particiones
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
source-git-commit: 4d4d87d2a03bc0966a6e77d97cb68a2c38a3c676
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Uso compartido de segmentaciones en espacios de trabajo y particiones {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Este artículo es solo para clientes que tienen espacios de trabajo y particiones.

## ¿Qué es una segmentación? {#whats-a-segmentation}

Marketo es bueno en elegir a las personas adecuadas para un programa o una campaña inteligente. Sin embargo, para perfiles más permanentes, debe utilizar segmentaciones. Son necesarios para utilizar contenido dinámico avanzado en Marketo.

>[!NOTE]
>
>Aprender [cómo crear segmentaciones](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Una vez configurados estos perfiles (_y_ Si utiliza espacios de trabajo), querrá compartirlos en los espacios de trabajo. Estas son algunas cosas buenas que hay que saber:

## Reglas y sugerencias {#rules-tips}

* Cada suscripción a Marketo puede contener hasta 20 segmentos en &quot;total&quot; en varios espacios de trabajo (**no 20 por espacio de trabajo**).
* Solo puede compartir una segmentación con espacios de trabajo a los que tenga acceso.
* Asegúrese de crear y utilizar un **Espacio de trabajo predeterminado con visibilidad en todas las particiones**.

* El procesamiento de la segmentación solo se ejecuta en las personas del espacio de trabajo en el que se ha creado.

   * Cree la segmentación que desee compartir en el espacio de trabajo predeterminado.
      * Aprobación de la segmentación
      * El espacio de trabajo compartido ve una carpeta bloqueada y la segmentación es de solo lectura.
      * No se puede editar la versión compartida. Solo puede editar la segmentación original en la que se creó.
   * Cuando hace clic en un segmento (p. ej., Asistencia sanitaria) dentro de una segmentación compartida, las personas que vea solo serán personas en la partición asociada al espacio de trabajo que esté viendo.
      * Si crea una segmentación en el espacio de trabajo 1 (WS1) y la comparte con WS2 y WS1 no tiene acceso a la partición para WS2, NO se volverá a calcular la segmentación.
      * Si crea una segmentación en un espacio de trabajo con particiones limitadas y, a continuación, la comparte con otro espacio de trabajo, ese espacio de trabajo que recibió la segmentación compartida solo verá a las personas si se superponen.


>[!NOTE]
>
>Algunas de estas reglas son un poco complejas. La forma más sencilla de empezar es realizar pruebas con personas específicas. Siempre puede realizar nuevas segmentaciones y deshacerse de las antiguas.

## Ejemplo de escenarios {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## Compartir una segmentación {#share-a-segmentation}

1. Vaya a la **Base de datos**.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Clic con el botón derecho **Segmentaciones** y seleccione **Nuevas carpetas**.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Asigne un nombre a la carpeta que va a compartir entre espacios de trabajo (ejemplo: Compartir segmentaciones).

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Mueva la segmentación que desee compartir a la carpeta.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Haga clic con el botón derecho en la carpeta y seleccione **Compartir carpeta**.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta. Clic **Guardar**.

   ![](assets/share-segmentations-across-workspaces-and-partitions.png)

   >[!NOTE]
   >
   >El cuadro de diálogo muestra los espacios de trabajo que tiene permiso para ver, por lo que Marketo recomienda crear y compartir Segmentaciones desde el espacio de trabajo predeterminado que tenga visibilidad de todos los espacios de trabajo y particiones.

La carpeta de origen se muestra en el árbol de la base de datos con una flecha que indica que se comparte con otros espacios de trabajo. Desde el espacio de trabajo compartido, la carpeta se muestra con un bloqueo para indicar que el contenido de la carpeta se ha compartido desde otro espacio de trabajo y es de solo lectura.
