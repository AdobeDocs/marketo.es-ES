---
unique-page-id: 10099680
description: Pasos para importar datos de objeto personalizados mediante un archivo CSV, incluida la selección del objeto personalizado, el modo de desduplicación y la asignación de campos.
title: Importar datos de objetos personalizables
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 4%

---

# Importar datos de objetos personalizables {#import-custom-object-data}

Es fácil importar datos de objeto personalizados en la base de datos. Si usa objetos personalizados con empresas, vea [Usar objetos personalizados con empresas](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) para obtener más información.

1. En Mi Marketo, vaya a **[!UICONTROL Base de datos]**.

   ![](assets/import-custom-object-data-1.png)

1. Haga clic en **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Importar datos de objeto personalizados]**.

   ![](assets/import-custom-object-data-2.png)

1. Haga clic en **[!UICONTROL Examinar]** para buscar el archivo de datos. Seleccione el formato de archivo (Valores separados por comas en este ejemplo).

   ![](assets/import-custom-object-data-3.png)

1. Seleccione su [!UICONTROL objeto personalizado].

   ![](assets/import-custom-object-data-4.png)

1. Seleccione [!UICONTROL Modo de desduplicación] de la lista desplegable. Haga clic en **[!UICONTROL Next]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilice los campos de desduplicación como identificadores únicos al crear o actualizar registros de objetos personalizados. Este ejemplo usa el campo Desduplicación del objeto personalizado **car**: vin (número de identificación del vehículo). Si solo está actualizando registros de objetos personalizados, puede seleccionar [!UICONTROL Marketo Guid] como [!UICONTROL Modo de desduplicación].

1. Asigne cada columna a un campo de Marketo, seleccionándolo en la lista desplegable.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Asegúrese de que los valores del archivo coincidan con el tipo de campo con el que los hace coincidir (por ejemplo, texto, entero, etc.); de lo contrario, el archivo se rechazará.

1. Haga clic en **[!UICONTROL Next]**.

   ![](assets/import-custom-object-data-7.png)

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >El límite de tamaño para los objetos personalizados es de 100 MB.

   >[!TIP]
   >
   >Escriba su dirección de correo electrónico en el campo **[!UICONTROL Enviar alerta a]** y Marketo le enviará un correo electrónico cuando finalice la importación.

1. En la esquina superior derecha de la pantalla, verá una notificación mientras se ejecuta la importación y los resultados finales cuando se complete.

   ![](assets/import-custom-object-data-9.png)

   ¡Yay!

>[!MORELIKETHIS]
>
>[Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
