---
unique-page-id: 7515767
description: Uso compartido de segmentaciones en espacios de trabajo y particiones - Documentos de Marketo - Documentación del producto
title: Uso compartido de segmentaciones en espacios de trabajo y particiones
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
feature: Partitions, Workspaces
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Uso compartido de segmentaciones en espacios de trabajo y particiones {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Este artículo es solo para clientes que tienen espacios de trabajo y particiones.

## ¿Qué es una segmentación? {#whats-a-segmentation}

Marketo es excelente para elegir a las personas adecuadas para un programa o una campaña inteligente. Sin embargo, para perfiles más permanentes, debe utilizar segmentaciones. Son necesarios para utilizar contenido dinámico avanzado en Marketo.

>[!NOTE]
>
>Aprenda [a crear segmentaciones](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Una vez que haya configurado estas personalidades (_y_ que usa espacios de trabajo), querrá compartirlas en los espacios de trabajo. Estas son algunas cosas buenas que hay que saber:

## Reglas y sugerencias {#rules-tips}

* Cada suscripción a Marketo puede contener hasta 20 segmentos en &quot;total&quot; en varios espacios de trabajo (**no 20 por espacio de trabajo**).
* Solo puede compartir una segmentación con espacios de trabajo a los que tenga acceso.
* Asegúrese de crear y utilizar un **espacio de trabajo predeterminado con visibilidad en todas las particiones**.

* El procesamiento de la segmentación solo se ejecuta en las personas del espacio de trabajo en el que se ha creado.

   * Cree la segmentación que desee compartir dentro de la Workspace predeterminada.
      * Aprobación de la segmentación
      * El espacio de trabajo compartido ve una carpeta bloqueada y la segmentación es de solo lectura.
      * No se puede editar la versión compartida. Solo puede editar la segmentación original en la que se creó.

   * Cuando hace clic en un segmento (p. ej., Asistencia sanitaria) dentro de una segmentación compartida, las personas que vea solo serán personas en la partición asociada al espacio de trabajo que esté viendo.
      * Si crea una segmentación en Workspace 1 (WS1) y la comparte con WS2 y WS1 no tiene acceso a la partición para WS2, NO se recalculará la segmentación.
      * Si crea una segmentación en un espacio de trabajo con particiones limitadas y, a continuación, la comparte con otro espacio de trabajo, ese espacio de trabajo que recibió la segmentación compartida solo verá a las personas si se superponen.

>[!NOTE]
>
>Algunas de estas reglas son un poco complejas. La forma más sencilla de empezar es realizar pruebas con personas específicas. Siempre puede realizar nuevas segmentaciones y deshacerse de las antiguas.

## Ejemplo de escenarios {#example-scenarios}

![](assets/share-segmentations-across-workspaces-and-partitions-1.png)

![](assets/share-segmentations-across-workspaces-and-partitions-2.png)

## Compartir una segmentación {#share-a-segmentation}

1. Ir a **[!UICONTROL Base de datos]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-3.png)

1. Haga clic con el botón derecho en **[!UICONTROL Segmentaciones]** y seleccione **[!UICONTROL Nueva carpeta]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-4.png)

1. Asigne un nombre a la carpeta que va a compartir en los espacios de trabajo (ejemplo: Compartir segmentaciones) y haga clic en **[!UICONTROL Crear]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-5.png)

1. Mueva la segmentación que desee compartir a la carpeta.

   ![](assets/share-segmentations-across-workspaces-and-partitions-6.png)

1. Haga clic con el botón derecho en la carpeta y seleccione **[!UICONTROL Compartir carpeta]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-7.png)

1. Seleccione los espacios de trabajo con los que desea compartir la carpeta. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-8.png)

   >[!NOTE]
   >
   >El cuadro de diálogo muestra los espacios de trabajo que tiene permiso para ver, por lo que Marketo recomienda crear y compartir Segmentaciones desde el espacio de trabajo predeterminado que tenga visibilidad de todos los espacios de trabajo y particiones.

La carpeta de origen se muestra en el árbol de la base de datos con una flecha que indica que se comparte con otros espacios de trabajo. Desde el espacio de trabajo compartido, la carpeta se muestra con un bloqueo para indicar que el contenido de la carpeta se ha compartido desde otro espacio de trabajo y es de solo lectura.
