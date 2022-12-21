---
unique-page-id: 10098379
description: 'Usar la sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado: Marketo Docs: documentación del producto'
title: Usar la sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Usar la sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing o ventas quiere un nuevo campo. O, tal vez olvidó uno en su selección inicial de campo. O bien, sus necesidades han cambiado. En cualquier caso, puede utilizar la sincronización rápida para volver a sincronizar campos específicos.

Normalmente, se utiliza la sincronización rápida para agregar un campo nuevo y se actualizan los valores. Sin embargo, hay casos en los que puede que desee sincronizar un campo existente. Puede restringir la sincronización de campos en función de un intervalo de fechas actualizado o creado. Consulte [Opciones de sincronización avanzadas](#Advanced_Sync_Options) a continuación para obtener más información.

La sincronización rápida puede sincronizar valores nulos. Por ejemplo, si está utilizando los valores A y B y cambia un valor B en Dynamics a null, sincronizará el valor nulo con Marketo.

## Sincronización rápida para todos los registros {#quick-sync-for-all-records}

A continuación se explica cómo utilizar la sincronización rápida para volver a sincronizar los campos nuevos.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Haga clic en **Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. En Detalles de sincronización de campos, haga clic en **Editar**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Seleccione los campos que desea sincronizar rápidamente y haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Puede seleccionar campos de varias entidades.

1. Recibirá una notificación cuando se complete la sincronización.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >La sincronización se ejecuta en paralelo con otras sincronizaciones y, según el tamaño de la base de datos, puede tardar mucho tiempo en completarse. Cuando un campo está en cola para su sincronización, no se puede anular la selección.

## Opciones de sincronización avanzadas {#advanced-sync-options}

¿Qué sucede si desea sincronizar un campo existente, pero solo lo hace para un conjunto limitado de datos? Así es como.

1. Desactive la casilla de verificación de un campo existente. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Vuelva a abrir la ventana emergente y vuelva a seleccionar el campo .

   ![](assets/select-field-reselect-hand.png)

1. Haga clic en **Sincronización avanzada**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Choose **Actualizado** y seleccione un intervalo de fechas utilizando los selectores de fechas. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Solo los registros actualizados entre el 19/8/16 y el 19/9/16 se sincronizarán rápidamente para el campo.

## Corrección de campos de sincronización {#fixing-out-of-sync-fields}

En el improbable caso de que un campo de Dynamics y Marketo no esté sincronizado, hay una forma rápida y sencilla de resincronizarlos.

1. Anule la selección del campo y haga clic en **Guardar**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Vuelva a seleccionar el campo y haga clic en **Guardar**. ¡Eso es todo!

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   ¡Eso debería arreglarlo!
