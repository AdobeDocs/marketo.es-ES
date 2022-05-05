---
description: Sincronización de objetos personalizados - Documentos de Marketo - Documentación del producto
title: Sincronización de objetos personalizados
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Sincronización de objetos personalizados {#custom-object-sync}

Los objetos personalizados creados en la instancia de Veeva CRM también pueden formar parte del Marketo Engage. A continuación se explica cómo configurarlo.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!PREREQUISITES]
>
>Para utilizar un objeto personalizado, debe estar asociado a un objeto de contacto o cuenta en Veva CRM.

## Habilitar objeto personalizado {#enable-custom-object}

1. En Marketo, haga clic en **Administrador**, luego **Sincronización de objetos de veeva**.

   ![](assets/custom-object-sync-1.png)

1. Si este es su primer objeto personalizado, haga clic en **Sincronizar esquema**.

   ![](assets/custom-object-sync-2.png)

1. Haga clic en **Deshabilitar sincronización global**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >La sincronización inicial del esquema de objeto personalizado de Veva puede tardar unos minutos.

1. Arrastre el objeto personalizado que desea sincronizar en el lienzo.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Los objetos personalizados deben tener nombres únicos. Marketo no admite dos objetos personalizados diferentes con el mismo nombre.

1. Haga clic en **Habilitar sincronización**.

   ![](assets/custom-object-sync-5.png)

1. Haga clic en **Habilitar sincronización** de nuevo.

   ![](assets/custom-object-sync-6.png)

1. Vuelva a la **Véeva** pestaña .

   ![](assets/custom-object-sync-7.png)

1. Haga clic en **Habilitar sincronización**.

   ![](assets/custom-object-sync-8.png)

1. Para ver todos los objetos personalizados de Veva, haga clic en Admin y Veva Objects Sync.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo solo admite entidades personalizadas vinculadas a entidades estándar con una profundidad de entre uno y dos niveles.

¡Excelente! Ahora puede utilizar datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>* [Sincronización de mensajes clave de llamada y de llamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
>* [Agregar o quitar un campo de objeto personalizado como restricciones de lista/Déclencheur inteligente](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}

