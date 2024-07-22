---
unique-page-id: 2953471
description: 'Sincronización de SFDC: sincronización de objetos personalizada - Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: sincronización de objetos personalizada'
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Sincronización SFDC: sincronización de objetos personalizada {#sfdc-sync-custom-object-sync}

Los objetos personalizados creados en su instancia de Salesforce también pueden formar parte de Marketo Engage. A continuación se muestra cómo configurarlo.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!PREREQUISITES]
>
>Para usar un objeto personalizado, debe estar asociado a un objeto [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"} o [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"} en Salesforce.

>[!IMPORTANT]
>
>El usuario de sincronización de Marketo necesita acceso de lectura al objeto personalizado para enumerarlo y realizar una sincronización con él.

## Habilitar objeto personalizado  {#enable-custom-object}

1. Haga clic en **[!UICONTROL Admin]** y en el vínculo **[!UICONTROL Sincronización de objetos de Salesforce]**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Si este es su primer objeto personalizado, haga clic en **[!UICONTROL Sincronizar esquema]**.

   ![](assets/rtaimage-2.png)

1. Haga clic en **[!UICONTROL Deshabilitar sincronización global]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Una sincronización inicial del esquema de objeto personalizado de Salesforce puede tardar unos minutos.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Arrastre el objeto personalizado que desee sincronizar al lienzo.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Los objetos personalizados deben tener nombres únicos. Marketo no admite dos objetos personalizados diferentes con el mismo nombre.

1. Haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Vuelva a hacer clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >No olvide volver a activar la sincronización global.

1. Vuelva a la ficha **Salesforce**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Para ver todos los objetos personalizados de Salesforce, haz clic en **[!UICONTROL Admin]** y en el vínculo **[!UICONTROL Sincronización de objetos de Salesforce]** (igual que el paso 1 anterior).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo solo admite entidades personalizadas vinculadas a entidades estándar de uno o dos niveles de profundidad.

### ¿Qué sigue? {#whats-next}

[Agregar o quitar campo de objeto personalizado como restricciones de lista inteligente/Déclencheur](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

¡Excelente! Ahora puede utilizar los datos de este objeto personalizado en campañas inteligentes y listas inteligentes.
