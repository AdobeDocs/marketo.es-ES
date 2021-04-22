---
unique-page-id: 4719297
description: Habilitar/Deshabilitar la sincronización de objetos personalizados - Documentos de Marketo - Documentación del producto
title: Habilitar/deshabilitar la sincronización de objetos personalizados
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Habilitar/deshabilitar la sincronización de objetos personalizados {#enable-disable-custom-object-sync}

Los objetos personalizados creados en la instancia de Salesforce también pueden formar parte de Marketo. Así es como configurarlo.

## Habilitar/deshabilitar la sincronización de objetos personalizados {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Se requieren derechos de administrador.

1. Haga clic en **Admin**.

   ![](assets/one.png)

1. En el menú Administración de bases de datos, haga clic en **Sincronización de objetos de Salesforce**.

   ![](assets/two-2.png)

1. Si este es su primer objeto personalizado, haga clic en **Sincronizar esquema.** De lo contrario, haga clic en  **Actualizar** esquema para asegurarse de que tiene la última versión.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Si se está ejecutando la sincronización global, tendrá que deshabilitarla haciendo clic en **Deshabilitar sincronización global.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La sincronización del esquema de objetos personalizados de Salesforce puede tardar unos minutos.

1. Haga clic en **Actualizar esquema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Seleccione el objeto que desea sincronizar y haga clic en **Habilitar sincronización**.

   >[!TIP]
   >
   >Marketo solo puede sincronizar un objeto personalizado si tiene una relación directa con el objeto posible cliente, contacto o cuenta de Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Haga clic **Habilitar sincronización** de nuevo.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Vuelva a la pestaña **Salesforce** y haga clic en **Habilitar sincronización**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Uso de los objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>No se pueden usar objetos personalizados en campañas inteligentes con déclencheur.

1. En la lista inteligente, arrastre el filtro **Tiene oportunidad** y configúrelo en **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. A continuación, utilice restricciones de filtro para reducir el enfoque.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   ¡Excelente! Ahora puede utilizar los datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>[Agregar o quitar un campo de objeto personalizado como restricciones de lista/Déclencheur inteligente](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
