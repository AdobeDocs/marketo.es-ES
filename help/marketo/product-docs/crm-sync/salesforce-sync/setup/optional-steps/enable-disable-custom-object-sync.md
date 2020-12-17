---
unique-page-id: 4719297
description: Activar/Desactivar la sincronización de objetos personalizados - Documentos de marketing - Documentación del producto
title: Activar/Desactivar sincronización de objetos personalizados
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Habilitar/Deshabilitar sincronización de objetos personalizados {#enable-disable-custom-object-sync}

Los objetos personalizados creados en la instancia de Salesforce también pueden formar parte de Marketing. Así es como configurarlo.

## Habilitar/Deshabilitar sincronización de objetos personalizados {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Se requieren derechos de administrador.

1. Haga clic en **Administración**.

   ** ![](assets/one.png)

   **

1. En el menú Administración de bases de datos, haga clic en **Salesforce** **Objetos Sincronizar**.

   ![](assets/two-2.png)

1. Si este es su primer objeto personalizado, haga clic en **Sincronizar esquema.** De lo contrario, haga clic en  **Actualizar** esquema para asegurarse de que dispone de la última versión.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Si se está ejecutando la sincronización global, tendrá que deshabilitarla haciendo clic en **Deshabilitar sincronización global.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La sincronización del esquema de objetos personalizados de Salesforce puede tardar unos minutos.

1. Haga clic en **Actualizar Esquema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Seleccione el objeto que desee sincronizar y haga clic en **Habilitar sincronización**.

   >[!TIP]
   >
   >Marketo sólo puede sincronizar un objeto personalizado si tiene una relación directa con el objeto Posible cliente, Contacto o Cuenta en Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Vuelva a hacer clic en **Habilitar la sincronización**.

   ** ![](assets/image2014-12-10-10-3a15-3a40.png)

   **

1. Vuelva a la ficha **Salesforce** y haga clic en **Habilitar sincronización**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Uso de los objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>No se pueden utilizar objetos personalizados en campañas inteligentes con activadores.

1. En la lista inteligente, arrastre el ratón sobre el filtro **Tiene oportunidad** y defina en **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. A continuación, utilice restricciones de filtro para reducir el enfoque.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   ¡Excelente! Ahora puede utilizar los datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>* [Añadir/quitar el campo de objeto personalizado como restricciones de Lista inteligente/activador](add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

>



