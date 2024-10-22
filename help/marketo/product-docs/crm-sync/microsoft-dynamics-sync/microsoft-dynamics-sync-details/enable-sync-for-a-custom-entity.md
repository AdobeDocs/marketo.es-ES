---
unique-page-id: 2953384
description: Habilitar la sincronización para una entidad personalizada - Documentos de Marketo - Documentación del producto
title: Habilitar sincronización para una entidad personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 79ae0d56dd4bb8bf563c6546cba54b89b5841425
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Habilitar sincronización para una entidad personalizada {#enable-sync-for-a-custom-entity}

Si necesita que los datos de entidad personalizados de Dynamics estén disponibles en Marketo Engage, así es como habilitar la sincronización.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>* Cuando se habilita la sincronización para una entidad personalizada, Marketo realiza una sincronización inicial para incluir todos los datos del objeto personalizado.
>* Los miembros de la lista de marketing y de la lista de marketing _no son compatibles_ en este momento.

>[!IMPORTANT]
>
>El usuario de sincronización de Marketo necesita acceso de lectura al objeto personalizado para enumerarlo y realizar una sincronización con él.

1. Vaya a la sección **[!UICONTROL Admin]**.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Seleccione **[!UICONTROL Microsoft Dynamics]** y haga clic en **[!UICONTROL Deshabilitar sincronización]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Debe deshabilitar la sincronización global temporalmente para habilitar o deshabilitar una entidad personalizada.

1. En Administración de bases de datos, haga clic en **[!UICONTROL Sincronizar entidades de Dynamics]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Haga clic en **[!UICONTROL Sincronizar esquema]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Seleccione la entidad que desea sincronizar y haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Seleccione los campos que desee sincronizar o usar como [restricciones](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) y/o déclencheur (para registros agregados, _no_ actualizados) en listas inteligentes. Cuando termine, haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante el proceso de sincronización, es posible que observe que el elemento &quot;[!UICONTROL Sincronización de entidades dinámicas]&quot; desaparece del árbol de navegación. Este es el comportamiento esperado y volverá a aparecer una vez completada la sincronización.

1. La entidad ahora tiene una marca de verificación verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. No olvide volver a activar la sincronización global.

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* Marketo solo admite entidades personalizadas vinculadas a entidades estándar de uno o dos niveles de profundidad.
   >
   >* El árbol de objetos personalizados puede mostrar el mismo objeto más de una vez, debido a sus conexiones directas con uno de los objetos principales (por ejemplo, posibles clientes, contactos o cuentas o conexiones indirectas a través de objetos intermediarios). En estos casos, elija el objeto más cercano al objeto principal y elija solo uno. Si elige el mismo objeto varias veces, puede que la sincronización de ese objeto personalizado se vea obstaculizada.
