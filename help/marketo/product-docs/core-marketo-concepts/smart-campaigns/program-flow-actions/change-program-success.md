---
unique-page-id: 1147009
description: Cambio del éxito del programa - Documentos de Marketo - Documentación del producto
title: Cambiar el éxito del programa
exl-id: 5b45b6d0-0c3d-4677-8b9a-8bbf03b1209e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 6%

---

# Cambiar el éxito del programa {#change-program-success}

## Resumen {#overview}

Si alguna vez tiene un grupo de personas marcadas por error con éxito del programa, puede utilizar este paso de flujo para establecer el éxito como verdadero o falso.

![](assets/image2014-9-22-14-3a45-3a8.png)

## Uso {#usage}

1. Cuando arrastre este paso de flujo, el programa se establecerá automáticamente en el programa que contenga la campaña inteligente que esté editando.

   >[!NOTE]
   >
   >Solo se verán afectados los miembros del programa.

   ![](assets/image2014-9-22-14-3a45-3a35.png)

1. Select **Correcto** o **Fecha de éxito** como atributo.

   ![](assets/image2014-9-22-14-3a45-3a39.png)

   >[!NOTE]
   >
   >Si establece Fecha de éxito en cualquier valor, automáticamente establece la métrica de éxito en verdadero. Si se establece Success en true , automáticamente se establece la Fecha de éxito en la fecha actual.

1. Configure las variables **Nuevo valor** a **True** o **False**.

   ![](assets/image2014-9-22-14-3a45-3a55.png)

   >[!TIP]
   >
   >Puede utilizar el paso de flujo dos veces para establecer tanto el indicador de éxito como la fecha.

¡Excelente! Ahora sabe cómo deshacer y forzar el éxito.
