---
unique-page-id: 4719297
description: Habilitar/Deshabilitar sincronización de objetos personalizada - Documentos de Marketo - Documentación del producto
title: Habilitar/Deshabilitar sincronización de objetos personalizada
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Habilitar/Deshabilitar sincronización de objetos personalizada {#enable-disable-custom-object-sync}

Los objetos personalizados creados en su instancia de Salesforce también pueden formar parte de Marketo Engage. A continuación se muestra cómo configurarlo.

## Habilitar/Deshabilitar sincronización de objetos personalizada {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Clic **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. En el menú Administración de bases de datos, haga clic en **[!UICONTROL Sincronización de objetos de Salesforce]**.

   ![](assets/two-2.png)

1. Si este es su primer objeto personalizado, haga clic en **[!UICONTROL Sincronizar esquema]**. De lo contrario, haga clic **[!UICONTROL Actualizar esquema]** para asegurarse de que dispone de la última versión.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Si la sincronización global se está ejecutando, tendrá que deshabilitarla haciendo clic en **[!UICONTROL Deshabilitar sincronización global]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Una sincronización del esquema de objeto personalizado de Salesforce puede tardar unos minutos.

1. Clic **[!UICONTROL Actualizar esquema]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Seleccione el objeto que desea sincronizar y haga clic en **[!UICONTROL Habilitar sincronización]**.

   >[!TIP]
   >
   >Marketo solo puede sincronizar un objeto personalizado si tiene una relación directa con el objeto Posible cliente, Contacto o Cuenta en Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Clic **[!UICONTROL Habilitar sincronización]** otra vez.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Vuelva a la **[!DNL Salesforce]** y haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Uso de los objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>No se pueden usar objetos personalizados en campañas inteligentes con déclencheur.

1. En la lista inteligente, arrastre el puntero sobre **[!UICONTROL Tiene oportunidad]** filtrar y establecer en **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. A continuación, utilice restricciones de filtro para reducir el enfoque.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   ¡Excelente! Ahora puede utilizar los datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>[Agregar o quitar campos de objetos personalizados como restricciones de listas inteligentes o Déclencheur](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
