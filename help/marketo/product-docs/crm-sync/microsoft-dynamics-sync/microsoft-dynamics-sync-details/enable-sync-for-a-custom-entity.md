---
unique-page-id: 2953384
description: Habilitar la sincronización para una entidad personalizada - Documentos de Marketo - Documentación del producto
title: Habilitar sincronización para una entidad personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Habilitar sincronización para una entidad personalizada {#enable-sync-for-a-custom-entity}

Si necesita que los datos de entidad personalizados de Dynamics estén disponibles en Marketo, así es como habilitar la sincronización.

>[!NOTE]
>
>**Permisos de administración necesarios**

>[!NOTE]
>
>* Cuando se habilita la sincronización para una entidad personalizada, Marketo realiza una sincronización inicial para incluir todos los datos del objeto personalizado.
>* Los miembros de la lista y la lista de marketing son **no admitido** en este momento.

>[!IMPORTANT]
>
>El usuario de sincronización de Marketo necesita acceso de lectura al objeto personalizado para enumerarlo y realizar una sincronización con él.

1. Vaya a la **Administrador** sección.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Seleccionar **Microsoft Dynamics** y haga clic en **Deshabilitar sincronización**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Debe deshabilitar la sincronización global temporalmente para habilitar o deshabilitar una entidad personalizada.

1. En Administración de bases de datos, haga clic en **Sincronización de entidades de Dynamics** vínculo.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Haga clic en **Sincronizar esquema** vínculo.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Seleccione la entidad que desee sincronizar y haga clic en **Habilitar sincronización**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Seleccione los campos que desee sincronizar o utilice como [restricciones](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) o déclencheur en listas inteligentes. Cuando termine, haga clic en **Habilitar sincronización**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante el proceso de sincronización, es posible que observe que el elemento &quot;Sincronización de entidades dinámicas&quot; desaparece del árbol de navegación. Este es el comportamiento esperado y volverá a aparecer una vez completada la sincronización.

1. La entidad ahora tiene una marca de verificación verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. No olvide volver a activar la sincronización global.

   ![](assets/enable-sync-for-a-custom-entity-8.png)
