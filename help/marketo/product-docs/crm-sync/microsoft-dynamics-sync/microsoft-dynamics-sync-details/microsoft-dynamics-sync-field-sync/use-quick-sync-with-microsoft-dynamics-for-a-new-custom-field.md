---
unique-page-id: 10098379
description: Aprenda a utilizar la sincronización rápida con Microsoft Dynamics al agregar un nuevo campo personalizado. Actualice los datos de campo de Dynamics a Marketo después de agregar el campo.
title: Utilizar la sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/Foo1CpTpWKCvtPTZv7NRuSoCvD18-x5OIABM48-UF6I
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 4%

---

# Usar sincronización rápida con [!DNL Microsoft Dynamics] para un nuevo campo personalizado {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing o Ventas desea un nuevo campo. O quizás olvidó uno en su selección inicial de campo. O, sus necesidades cambiaron. En cualquier caso, puede utilizar la sincronización rápida para volver a sincronizar campos específicos.

Normalmente, la sincronización rápida se utiliza para agregar un nuevo campo y actualizar los valores. Sin embargo, hay casos en los que es posible que desee sincronizar un campo existente. Puede restringir la sincronización de campos en función de un intervalo de fechas actualizado o creado. Consulte [Opciones de sincronización avanzadas](#Advanced_Sync_Options) más abajo para obtener más información.

La sincronización rápida puede sincronizar valores nulos. Por ejemplo, si está utilizando los valores A y B y cambia el valor B de [!DNL Dynamics] a nulo, sincronizará el valor nulo con Marketo.

## Sincronización rápida para todos los registros {#quick-sync-for-all-records}

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Haga clic en **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. En [!UICONTROL Detalles de sincronización de campos], haga clic en **[!UICONTROL Editar]**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Seleccione los campos que desea sincronizar rápidamente y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Puede seleccionar campos de varias entidades.

1. Recibirá una notificación cuando se complete la sincronización.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >La sincronización se ejecuta en paralelo con otras sincronizaciones y, según el tamaño de la base de datos, puede tardar mucho tiempo en completarse. Cuando un campo está en cola para sincronizarse, no se puede anular su selección.

## Opciones de sincronización avanzadas {#advanced-sync-options}

¿Qué sucede si desea sincronizar un campo existente pero solo lo hace para un conjunto limitado de datos?

1. Desactive la casilla de verificación de un campo existente. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Vuelva a abrir la ventana emergente y vuelva a seleccionar el campo.

   ![](assets/select-field-reselect-hand.png)

1. Haga clic en **[!UICONTROL Sincronización avanzada]**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Elija **[!UICONTROL Actualizado]** y seleccione un intervalo de fechas utilizando los selectores de fechas. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Solo se sincronizarán rápidamente los registros actualizados entre el 19/8/16 y el 19/9/16 para el campo.

## Corrección de campos no sincronizados {#fixing-out-of-sync-fields}

En el improbable caso de que un campo de [!DNL Dynamics] y Marketo no estén sincronizados, existe una forma rápida de volver a sincronizarlos.

1. Anule la selección del campo y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Vuelva a seleccionar el campo y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   ¡Eso debería arreglarlo!
