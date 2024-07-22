---
description: Habilitar/Deshabilitar sincronización de objetos personalizada - Documentos de Marketo - Documentación del producto
title: Habilitar/Deshabilitar sincronización de objetos personalizada
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Habilitar/Deshabilitar sincronización de objetos personalizada {#enable-disable-custom-object-sync}

Los objetos personalizados creados en su instancia de Veeva CRM también pueden formar parte de Marketo Engage. A continuación se muestra cómo configurarlo.

## Habilitar o deshabilitar la sincronización de objetos personalizada {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. En Marketo, haz clic en **[!UICONTROL Administrador]** y luego en **[!UICONTROL Sincronizar objetos de Veeva]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Si este es su primer objeto personalizado, haga clic en Sincronizar esquema. Si no es así, haga clic en **[!UICONTROL Actualizar esquema]** para asegurarse de que dispone de la última versión.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Si la sincronización global se está ejecutando, desactívela haciendo clic en **[!UICONTROL Deshabilitar sincronización global]**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Una sincronización del esquema de objeto personalizado de Veeva puede tardar unos minutos.

1. Haga clic en **[!UICONTROL Actualizar esquema]**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Seleccione el objeto que desea sincronizar y haga clic en Habilitar sincronización.

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo solo puede sincronizar un objeto personalizado si tiene una relación directa con el objeto Contacto o Cuenta en Veeva CRM.

1. Vuelva a hacer clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Vuelva a la ficha Veeva y haga clic en **[!UICONTROL Habilitar sincronización]**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Uso de los objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>No se pueden usar objetos personalizados en campañas inteligentes con déclencheur.

1. En la lista inteligente, arrastre el cursor sobre el filtro &quot;Tiene oportunidad&quot; y establezca en **[!UICONTROL True]**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. De forma opcional, utilice restricciones de filtro para reducir el enfoque.

   ![](assets/enable-disable-custom-object-sync-9.png)

¡Excelente! Ahora puede utilizar los datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>[Agregar o quitar campo de objeto personalizado como restricciones de lista inteligente/Déclencheur](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
