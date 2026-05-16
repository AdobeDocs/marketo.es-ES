---
unique-page-id: 4719297
description: Obtenga información sobre cómo habilitar o deshabilitar la sincronización de objetos personalizados de Salesforce en Marketo Engage. Utilice Admin y Salesforce Objects Sync para seleccionar objetos y actualizar el esquema.
title: Habilitar/deshabilitar sincronización de objetos personalizada
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/QdXTpcTi0eQKk8flu8HxHhaK2sEO4JRkeehq3KxDRo0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399
subfeature_v2: id: d0251300-e25f-466f-9856-7e11ce8fa7aa
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 234
ht-degree: 6%

---

# Habilitar/deshabilitar sincronización de objetos personalizada {#enable-disable-custom-object-sync}

Los objetos personalizados creados en su instancia de Salesforce también pueden formar parte de Marketo Engage. A continuación se muestra cómo configurarlo.

## Habilitar/deshabilitar sincronización de objetos personalizada {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. En el menú Administración de bases de datos, haga clic en **[!UICONTROL Sincronizar objetos de Salesforce]**.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Si este es su primer objeto personalizado, haga clic en **[!UICONTROL Sincronizar esquema]**. De lo contrario, haga clic en **[!UICONTROL Actualizar esquema]** para asegurarse de que dispone de la última versión.

   ![](assets/enable-disable-custom-object-sync-3.png)

1. Si la sincronización global se está ejecutando, tendrá que deshabilitarla haciendo clic en **[!UICONTROL Deshabilitar sincronización global]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Una sincronización del esquema de objeto personalizado [!DNL Salesforce] puede tardar unos minutos.

1. Haga clic en **[!UICONTROL Actualizar esquema]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Seleccione el objeto que desea sincronizar y haga clic en **[!UICONTROL Habilitar sincronización]**.

   >[!TIP]
   >
   >Marketo solo puede sincronizar un objeto personalizado si tiene una relación directa con el objeto de posible cliente, contacto o cuenta en [!DNL Salesforce].

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Vuelva a hacer clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Vuelva a la ficha **[!DNL Salesforce]** y haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Uso de los objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>No se pueden usar objetos personalizados en campañas inteligentes con déclencheur.

1. En tu lista inteligente, arrastra el filtro **[!UICONTROL Tiene oportunidad]** y establece en **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. A continuación, utilice restricciones de filtro para reducir el enfoque.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Ahora puede utilizar los datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>[Agregar o quitar campo de objeto personalizado como restricciones de lista inteligente/Déclencheur](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
