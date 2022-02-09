---
unique-page-id: 2953384
description: Habilitar la sincronización para una entidad personalizada - Documentos de Marketo - Documentación del producto
title: Habilitar la sincronización para una entidad personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: dadaf5bd8e887309d0e9ee8fc25fc58d1c4fbe97
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# Habilitar la sincronización para una entidad personalizada {#enable-sync-for-a-custom-entity}

Si necesita que los datos de entidad personalizados de Dynamics estén disponibles en Marketo, así es como habilitarlos para la sincronización.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>* Al habilitar la sincronización para una entidad personalizada, Marketo realiza una sincronización inicial para incorporar todos los datos del objeto personalizado.
>* Los miembros de la Lista de marketing y la Lista de marketing son **no admitido** en este momento.


1. Vaya a la **Administrador** para obtener más información.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Select **Microsoft Dynamics** y haga clic en **Desactivar sincronización**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Debe desactivar la sincronización global temporalmente para habilitar o deshabilitar una entidad personalizada.

1. En Administración de bases de datos, haga clic en la **Sincronización de entidades de Dynamics** vínculo.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Haga clic en el **esquema de sincronización** vínculo.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Seleccione la entidad que desea sincronizar y haga clic en **Habilitar sincronización**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Seleccione los campos que desee sincronizar o utilizar como [restricciones](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) y/o déclencheur en listas inteligentes. Cuando termine, haga clic en **Habilitar sincronización**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante el proceso de sincronización, es posible que observe que el elemento &quot;Sincronización de entidades dinámicas&quot; desaparece del árbol de navegación. Esto es un comportamiento esperado y reaparecerá una vez finalizada la sincronización.

1. La entidad ahora tiene una marca de verificación verde en ella.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. No olvide volver a habilitar la sincronización global.

   ![](assets/enable-sync-for-a-custom-entity-8.png)
