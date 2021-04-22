---
unique-page-id: 2953471
description: Sincronización SFDC - Sincronización de objetos personalizados - Documentos de Marketo - Documentación del producto
title: Sincronización SFDC - Sincronización de objetos personalizados
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Sincronización SFDC: Sincronización de objetos personalizados {#sfdc-sync-custom-object-sync}

Los objetos personalizados creados en la instancia de Salesforce también pueden formar parte de Marketo.  Así es como configurarlo.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!PREREQUISITES]
>
>Para utilizar un objeto personalizado, debe estar asociado a un objeto [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md) o [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) en Salesforce.

## Habilitar objeto personalizado {#enable-custom-object}

1. Haga clic en **Admin** y en el enlace **Sincronización de objetos de Salesforce**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Si este es su primer objeto personalizado, haga clic en **Sincronizar esquema**.

   ![](assets/rtaimage-2.png)

1. Haga clic en **Deshabilitar sincronización global**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >La sincronización inicial del esquema de objetos personalizados de Salesforce puede tardar unos minutos.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Arrastre el objeto personalizado que desea sincronizar en el lienzo.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Los objetos personalizados deben tener nombres únicos. Marketo no admite dos objetos personalizados diferentes con el mismo nombre.

1. Haga clic en **Habilitar sincronización**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Haga clic **Habilitar sincronización** de nuevo.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >No olvide volver a habilitar la sincronización global.

1. Vuelva a la pestaña **Salesforce**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Haga clic en **Habilitar sincronización**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Para ver todos los objetos personalizados de Salesforce, haga clic en **Admin** y en el enlace **Sincronización de objetos de Salesforce** (igual que el paso 1 anterior).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo solo admite entidades personalizadas vinculadas a entidades estándar con una o dos niveles de profundidad.

### Siguientes pasos: {#whats-next}

[Agregar o quitar un campo de objeto personalizado como restricciones de lista/Déclencheur inteligente](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

¡Excelente! Ahora puede utilizar datos de este objeto personalizado en campañas inteligentes y listas inteligentes.
