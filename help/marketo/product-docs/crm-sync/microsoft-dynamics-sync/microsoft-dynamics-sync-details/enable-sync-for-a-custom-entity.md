---
unique-page-id: 2953384
description: Obtenga información sobre cómo habilitar la sincronización para una entidad personalizada en Microsoft Dynamics y Marketo. Use Administración y Microsoft Dynamics para seleccionar y habilitar entidades personalizadas para la sincronización.
title: Habilitar sincronización para una entidad personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/kSLFdQA9OTHLoBTQ2qBrRFucLaDJLNSNAxGqjjMHCxs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 329
ht-degree: 3%

---

# Habilitar sincronización para una entidad personalizada {#enable-sync-for-a-custom-entity}

Si necesita que los datos de entidad personalizados de [!DNL Dynamics] estén disponibles en Marketo Engage, siga los pasos a continuación.

>[!PREREQUISITES]
>
>Para usar un objeto personalizado, debe estar asociado a un objeto [lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md){target="_blank"} o [account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md){target="_blank"} en Microsoft Dynamics.

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

1. En [!UICONTROL Administración de bases de datos], haga clic en el vínculo **[!UICONTROL Sincronizar entidades de Dynamics]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Haga clic en el vínculo **[!UICONTROL Sincronizar esquema]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Seleccione la entidad que desea sincronizar y haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Seleccione los campos que desee sincronizar o usar como [restricciones](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) o déclencheur en listas inteligentes. Cuando termine, haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante el proceso de sincronización, es posible que observe que el elemento &quot;[!UICONTROL Sincronización de entidades dinámicas]&quot; desaparece del árbol de navegación. Este es el comportamiento esperado y volverá a aparecer una vez completada la sincronización.

1. La entidad ahora tiene una marca de verificación verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Vuelva a habilitar la sincronización global.

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* Marketo solo admite entidades personalizadas vinculadas a entidades estándar de uno o dos niveles de profundidad.
   >
   >* El árbol de objetos personalizados puede mostrar el mismo objeto más de una vez, debido a sus conexiones directas con uno de los objetos principales (por ejemplo, posibles clientes, contactos o cuentas o conexiones indirectas a través de objetos intermediarios). En estos casos, elija el objeto más cercano al objeto principal y elija solo uno. Si elige el mismo objeto varias veces, puede que la sincronización de ese objeto personalizado se vea obstaculizada.
