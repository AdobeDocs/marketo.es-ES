---
unique-page-id: 3571846
description: Microsoft Dynamics Sync - Sincronización de entidades personalizadas - Documentos de marketing - Documentación del producto
title: Microsoft Dynamics Sync - Sincronización de entidades personalizadas
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronización de entidad personalizada {#microsoft-dynamics-sync-custom-entity-sync}

Si necesita habilitar la sincronización de entidad personalizada inicial para que los datos de Dynamics estén disponibles en Marketing Cloud, así se explica cómo hacerlo.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>**Requisitos previos**
>
>Para utilizar un objeto personalizado, debe asociarse a un [objeto de posible cliente](microsoft-dynamics-sync-lead-sync.md), [contacto](microsoft-dynamics-sync-contact-sync.md)o [](microsoft-dynamics-sync-account-sync.md)cuenta en Dynamics.

>[!CAUTION]
>
>Asegúrese de completar la sincronización inicial (se le notificará por correo electrónico) antes de comenzar la sincronización para entidades personalizadas.

1. Vaya a la sección Administración.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Haga clic en **Deshabilitar sincronización** para deshabilitar temporalmente la sincronización global estándar.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Instale una versión de Microsoft Dynamics que admita la sincronización de entidades personalizada (después de 2_0_0_2). Consulte Versiones [del complemento de marketing para MIcrosoft Dynamics](../../../../product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).
1. Proporcione al usuario de sincronización de marketing acceso de lectura a todas las entidades que desee sincronizar.
1. En Administración de bases de datos, haga clic en el vínculo** Sincronización de entidades de Dynamics**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Haga clic en el vínculo **Sincronizar esquema** para recuperar la lista de las entidades personalizadas disponibles.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Después de sincronizar la lista, seleccione los campos que desee sincronizar y los que desee utilizar como [restricciones](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) o activadores en listas inteligentes. Cuando termine, haga clic en **Activar sincronización**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. Vuelva a habilitar la sincronización global.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketo solo admite entidades personalizadas que están vinculadas a entidades estándar de uno o dos niveles de profundidad.

   >[!NOTE]
   >
   >Los nombres de entidad pueden tener un máximo de** 33 caracteres**.

¡Estás bien!