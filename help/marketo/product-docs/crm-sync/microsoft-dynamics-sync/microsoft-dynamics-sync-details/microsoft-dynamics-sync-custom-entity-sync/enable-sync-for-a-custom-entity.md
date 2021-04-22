---
unique-page-id: 2953384
description: Habilitar la sincronización para una entidad personalizada - Documentos de Marketo - Documentación del producto
title: Habilitar la sincronización para una entidad personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Habilitar la sincronización para una entidad personalizada {#enable-sync-for-a-custom-entity}

Si necesita que los datos de entidad personalizados de Dynamics estén disponibles en Marketo, así es como habilitarlos:

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Vaya a la sección **Admin**.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Seleccione **Microsoft Dynamics** y haga clic en **Deshabilitar sincronización**.

   Debe desactivar la sincronización global temporalmente para habilitar o deshabilitar una entidad personalizada.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. En Administración de bases de datos, haga clic en el enlace **Sincronización de entidades de Dynamics**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Haga clic en el enlace **Sync schema**.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Seleccione la entidad que desea sincronizar y haga clic en **Habilitar sincronización**.

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. Seleccione los campos que desee sincronizar o utilizar como [restricciones](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) y/o déclencheur en listas inteligentes. Cuando termine, haga clic en **Habilitar sincronización**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >Durante el proceso de sincronización, es posible que observe que el elemento &quot;Sincronización de entidades dinámicas&quot; desaparece del árbol de navegación. Esto es un comportamiento esperado y reaparecerá una vez finalizada la sincronización.

1. La entidad ahora tiene una marca de verificación verde en ella.

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. No olvide volver a habilitar la sincronización global.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

¡Oh sí! Poderosas cosas.
