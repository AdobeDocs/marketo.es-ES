---
unique-page-id: 10099680
description: 'Importar Datos De Objetos Personalizados: Documentos De Marketo: Documentación Del Producto'
title: Importar datos de objeto personalizados
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Importar datos de objeto personalizados {#import-custom-object-data}

Es fácil importar datos de objetos personalizados en la base de datos. Si utiliza objetos personalizados con empresas, consulte [Uso de objetos personalizados con compañías](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) para obtener más información.

1. En Mi Marketo, vaya a **Base de datos**.

   ![](assets/import-custom-object-data-1.png)

1. Haga clic en **Nuevo** y seleccione **Importar datos de objeto personalizados**.

   ![](assets/import-custom-object-data-2.png)

1. Haga clic en **Examinar** para localizar el archivo de datos. Seleccione el formato de archivo (Valores separados por comas en este ejemplo).

   ![](assets/import-custom-object-data-3.png)

1. Seleccione el objeto personalizado.

   ![](assets/import-custom-object-data-4.png)

1. Seleccione el Modo de desduplicación en la lista desplegable. Haga clic en **Siguiente**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilice los campos de desduplicación como identificadores únicos al crear o actualizar registros de objeto personalizados. En este ejemplo se utiliza el campo Dedupe de la variable **car** custom object - vin (número de identificación del vehículo). Si solo está actualizando registros de objeto personalizados, puede seleccionar la guía de Marketo como modo de desduplicación.

1. Asigne cada columna a un campo de Marketo, seleccionándolo en la lista desplegable.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Asegúrese de que los valores del archivo coinciden con el tipo de campo al que los está haciendo coincidir (por ejemplo, texto, entero, etc.); de lo contrario, el archivo se rechazará.

1. Haga clic en **Siguiente**.

   ![](assets/import-custom-object-data-7.png)

1. Haga clic en **Importar**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >El límite de tamaño para los objetos personalizados es de 100 MB.

   >[!TIP]
   >
   >Escriba su dirección de correo electrónico en la **Enviar alerta a:** y Marketo le enviará un correo electrónico cuando haya terminado la importación.

1. En la esquina superior derecha de la pantalla, verá una notificación mientras se ejecuta la importación y los resultados finales cuando finalice.

   ![](assets/import-custom-object-data-9.png)

   ¡Sí!

>[!MORELIKETHIS]
>
>[Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
