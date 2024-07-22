---
description: Sincronización de objetos personalizados - Documentos de Marketo - Documentación del producto
title: Sincronización de objetos personalizados
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Sincronización de objetos personalizados {#custom-object-sync}

Los objetos personalizados creados en su instancia de Veeva CRM también pueden formar parte de Marketo Engage. A continuación se muestra cómo configurarlo.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!PREREQUISITES]
>
>Para utilizar un objeto personalizado, debe estar asociado a un objeto de contacto o cuenta en Veeva CRM.

## Habilitar objeto personalizado {#enable-custom-object}

1. En Marketo, haz clic en **[!UICONTROL Administrador]** y luego en **[!UICONTROL Sincronizar objetos de Veeva]**.

   ![](assets/custom-object-sync-1.png)

1. Si este es su primer objeto personalizado, haga clic en **[!UICONTROL Sincronizar esquema]**.

   ![](assets/custom-object-sync-2.png)

1. Haga clic en **[!UICONTROL Deshabilitar sincronización global]**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >La sincronización inicial del esquema de objeto personalizado de Veeva puede tardar unos minutos.

1. Arrastre el objeto personalizado que desee sincronizar al lienzo.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Los objetos personalizados deben tener nombres únicos. Marketo no admite dos objetos personalizados diferentes con el mismo nombre.

1. Haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/custom-object-sync-5.png)

1. Vuelva a hacer clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/custom-object-sync-6.png)

1. Vuelva a la ficha **[!UICONTROL Veeva]**.

   ![](assets/custom-object-sync-7.png)

1. Haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/custom-object-sync-8.png)

1. Para ver todos los objetos personalizados de Veeva, haz clic en **[!UICONTROL Administrador]** y **[!UICONTROL Sincronizar objetos de Veeva]**.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo solo admite entidades personalizadas vinculadas a entidades estándar de uno a dos niveles de profundidad.

¡Excelente! Ahora puede utilizar datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>* [Sincronizando mensajes de clave de llamada y llamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Agregar o quitar campo de objeto personalizado como restricciones de lista inteligente/Déclencheur](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
