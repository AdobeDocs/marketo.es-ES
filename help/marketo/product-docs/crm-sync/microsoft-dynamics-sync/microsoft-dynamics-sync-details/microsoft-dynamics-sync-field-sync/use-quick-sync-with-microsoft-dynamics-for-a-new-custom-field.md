---
unique-page-id: 10098379
description: Usar sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado - Documentos de marketing - Documentación del producto
title: Usar sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Usar sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing o ventas quiere un nuevo campo. O quizás olvidó uno en la selección inicial de campo. O bien, sus necesidades cambiaron. En cualquier caso, puede utilizar la sincronización rápida para resincronizar campos específicos.

Normalmente, usará la sincronización rápida para agregar un nuevo campo y actualizar los valores. Sin embargo, hay casos en los que puede que desee sincronizar un campo existente. Puede restringir la sincronización de campos en función de un intervalo de fechas actualizado o creado. Consulte Opciones [de sincronización](#Advanced_Sync_Options) avanzadas a continuación para obtener más información.

La sincronización rápida puede sincronizar valores nulos. Por ejemplo, si utiliza los valores A y B y cambia un valor B en Dynamics a null, sincronizará el valor nulo con Marketing.

## Sincronización rápida para todos los registros {#quick-sync-for-all-records}

A continuación se explica cómo utilizar la sincronización rápida para volver a sincronizar los campos nuevos.

1. En Marketing, haga clic en **Administración**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Haga clic en** Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. En Detalles de sincronización de campos, haga clic en **Editar**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Seleccione los campos para sincronizar rápidamente y haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Puede seleccionar campos de varias entidades.

1. Recibirá una notificación cuando se complete la sincronización.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >La sincronización se ejecuta en paralelo con otras sincronizaciones y, en función del tamaño de la base de datos, puede tardar mucho tiempo en completarse. Cuando un campo se encuentra en la cola para la sincronización, no se puede anular la selección.

## Opciones de sincronización avanzadas {#advanced-sync-options}

¿Qué sucede si desea sincronizar un campo existente, pero solo lo hace para un conjunto limitado de datos? Así es como.

1. Desactive la casilla de verificación de un campo existente. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Vuelva a abrir la ventana emergente y seleccione de nuevo el campo.

   ![](assets/select-field-reselect-hand.png)

1. Haga clic en Sincronización **avanzada**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Elija **Actualizado **y seleccione un intervalo de fechas con los selector de fechas. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Solo se sincronizarán rápidamente los registros actualizados entre el 19/8/16 y el 19/9/16 para el campo.

## Corrección de los campos de sincronización {#fixing-out-of-sync-fields}

En el caso poco frecuente de que un campo Dinámica y Marketing no estén sincronizados, hay una manera rápida y fácil de resincronizarlos.

1. Anule la selección del campo y haga clic en **Guardar**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Vuelva a seleccionar el campo y haga clic en **Guardar**. ¡Eso es todo!

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   ¡Eso debería arreglarlo!

