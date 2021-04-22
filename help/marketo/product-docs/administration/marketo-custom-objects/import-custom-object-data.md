---
unique-page-id: 10099680
description: 'Importar Datos De Objetos Personalizados: Documentos De Marketo: Documentación Del Producto'
title: Importar datos de objeto personalizados
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Importar datos de objeto personalizados {#import-custom-object-data}

Es fácil importar datos de objetos personalizados en la base de datos. Si utiliza objetos personalizados con empresas, consulte [Uso de objetos personalizados con compañías](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) para obtener más información.

1. En Mi Marketo, vaya a **Database**.

   ![](assets/db-1.png)

1. Haga clic en **Nuevo** y seleccione **Importar datos de objeto personalizados**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Haga clic en **Examinar** para localizar el archivo de datos. Seleccione el formato de archivo (Valores separados por comas en este ejemplo).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Seleccione el objeto personalizado.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Seleccione el Modo de desduplicación en la lista desplegable. Haga clic en **Siguiente**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Utilice los campos de desduplicación como identificadores únicos al crear o actualizar registros de objeto personalizados. Este ejemplo utiliza el campo Dedupe del **car** objeto personalizado: vin (número de ID del vehículo). Si solo está actualizando registros de objeto personalizados, puede seleccionar la guía de Marketo como modo de desduplicación.

1. Asigne cada columna a un campo de Marketo, seleccionándolo en la lista desplegable.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Asegúrese de que los valores del archivo coinciden con el tipo de campo al que los está haciendo coincidir (por ejemplo, texto, entero, etc.); de lo contrario, el archivo se rechazará.

1. Haga clic en **Siguiente**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Haga clic en **Import**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >El límite de tamaño para los objetos personalizados es de 100 MB.

   >[!TIP]
   >
   >Introduzca su dirección de correo electrónico en el campo **Send Alert To:** y Marketo le enviará un correo electrónico cuando termine la importación.

1. En la esquina superior derecha de la pantalla, verá una notificación mientras se ejecuta la importación y los resultados finales cuando finalice.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   ¡Sí!

>[!MORELIKETHIS]
>
>[Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
