---
unique-page-id: 10099680
description: Importar datos de objeto personalizados - Documentos de marketing - Documentación de producto
title: Importar datos de objeto personalizados
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Importar datos de objeto personalizados {#import-custom-object-data}

Es fácil importar datos de objetos personalizados en la base de datos. Si utiliza objetos personalizados con compañías, consulte [Uso de objetos personalizados con Compañías](http://docs.marketo.com/display/DOCS/Understanding+Marketo+Custom+Objects#UnderstandingMarketoCustomObjects-customcompanyUsingCustomObjectswithCompanies) para obtener más información.

1. En Mi marketing, vaya a **Base de datos**.

   ![](assets/db-1.png)

1. Haga clic en **Nuevo** y seleccione **Importar datos** de objeto personalizados.

   ![](assets/image2016-4-7-10-6-54.png)

1. Haga clic en **Examinar** para localizar el archivo de datos. Seleccione el formato de archivo (Valores separados por comas en este ejemplo).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Seleccione el objeto personalizado.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Seleccione el modo de desduplicación en la lista desplegable. Haga clic en **Siguiente**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Utilice los campos Desduplicación como identificadores únicos al crear o actualizar registros de objetos personalizados. En este ejemplo se utiliza el campo Dedupe del objeto personalizado **car** : vin (número de identificación del vehículo). Si solo está actualizando registros de objetos personalizados, puede seleccionar la Guía de marketing como modo de depuración.

1. Asigne cada columna a un campo de marketing, seleccionándolo en la lista desplegable.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Asegúrese de que los valores del archivo coincidan con el tipo de campo al que los hace coincidir (por ejemplo, texto, entero, etc.); de lo contrario, el archivo será rechazado.

1. Haga clic en **Siguiente**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Haga clic en **Importar**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >El límite de tamaño de los objetos personalizados es de 100 MB.

   >[!TIP]
   >
   >Escriba su dirección de correo electrónico en **Enviar alerta a:** y Marketing le enviarán un correo electrónico cuando finalice la importación.

1. En la esquina superior derecha de la pantalla, verá una notificación mientras se ejecuta la importación y los resultados finales cuando se complete.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   ¡Sí!

>[!MORELIKETHIS]
>
>* [Explicación de los objetos personalizados de marketing](understanding-marketo-custom-objects.md)

>



