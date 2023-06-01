---
unique-page-id: 10099680
description: Importar datos de objeto personalizados - Documentos de Marketo - Documentación del producto
title: Importar datos de objeto personalizados
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 4a33b192cc22550c75769b383e261ac0a86e7ddb
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Importar datos de objeto personalizados {#import-custom-object-data}

Es fácil importar datos de objeto personalizados en la base de datos. Si utiliza objetos personalizados con empresas, consulte [Uso de objetos personalizados con compañías](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) para obtener más información.

1. En Mi Marketo, vaya a **[!UICONTROL Base de datos]**.

   ![](assets/import-custom-object-data-1.png)

1. Clic **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Importar datos de objeto personalizados]**.

   ![](assets/import-custom-object-data-2.png)

1. Clic **[!UICONTROL Examinar]** para localizar el archivo de datos. Seleccione el formato de archivo (Valores separados por comas en este ejemplo).

   ![](assets/import-custom-object-data-3.png)

1. Seleccione su [!UICONTROL objeto personalizado].

   ![](assets/import-custom-object-data-4.png)

1. Seleccione el [!UICONTROL Modo de desduplicación] de la lista desplegable. Clic **[!UICONTROL Siguiente]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilice los campos de desduplicación como identificadores únicos al crear o actualizar registros de objetos personalizados. Este ejemplo utiliza el campo Dedupe del **coche** objeto personalizado - vin (número de identificación del vehículo). Si sólo está actualizando registros de objetos personalizados, puede seleccionar la opción [!UICONTROL Marketo Guid] como el [!UICONTROL Modo de desduplicación].

1. Asigne cada columna a un campo de Marketo, seleccionándolo en la lista desplegable.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Asegúrese de que los valores del archivo coincidan con el tipo de campo con el que los hace coincidir (por ejemplo, texto, entero, etc.); de lo contrario, el archivo se rechazará.

1. Clic **[!UICONTROL Siguiente]**.

   ![](assets/import-custom-object-data-7.png)

1. Clic **[!UICONTROL Importar]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >El límite de tamaño para los objetos personalizados es de 100 MB.

   >[!TIP]
   >
   >Introduzca su dirección de correo electrónico en la **[!UICONTROL Enviar alerta a]** y Marketo le enviarán un correo electrónico cuando haya finalizado la importación.

1. En la esquina superior derecha de la pantalla, verá una notificación mientras se ejecuta la importación y los resultados finales cuando se complete.

   ![](assets/import-custom-object-data-9.png)

   ¡Yay!

>[!MORELIKETHIS]
>
>[Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
