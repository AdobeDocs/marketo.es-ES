---
description: Habilitar/Deshabilitar la sincronización de objetos personalizados - Documentos de Marketo - Documentación del producto
title: Habilitar/deshabilitar la sincronización de objetos personalizados
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Habilitar/deshabilitar la sincronización de objetos personalizados {#enable-disable-custom-object-sync}

Los objetos personalizados creados en la instancia de Veeva CRM también pueden formar parte del Marketo Engage. A continuación se explica cómo configurarlo.

## Habilitar o deshabilitar la sincronización de objetos personalizados {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. En Marketo, haga clic en **Administrador**, luego **Sincronización de objetos de veeva**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Si este es su primer objeto personalizado, haga clic en Sincronizar esquema. Si no es así, haga clic en **Actualizar esquema** para asegurarse de que dispone de la última versión.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Si se está ejecutando la sincronización global, deshabilite la sincronización haciendo clic en **Deshabilitar sincronización global**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >La sincronización del esquema de objeto personalizado de Veva puede tardar unos minutos.

1. Haga clic en **Actualizar esquema**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Seleccione el objeto que desea sincronizar y haga clic en Activar sincronización.

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo solo puede sincronizar un objeto personalizado si tiene una relación directa con el objeto Contact o Account en Veva CRM.

1. Haga clic en **Habilitar sincronización** de nuevo.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Vuelva a la pestaña Veva y haga clic en **Habilitar sincronización**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Uso de objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>No se pueden usar objetos personalizados en campañas inteligentes con déclencheur.

1. En la lista inteligente, arrastre el filtro &quot;Tiene oportunidad&quot; y configúrelo en **True**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Opcionalmente, use restricciones de filtro para reducir el foco.

   ![](assets/enable-disable-custom-object-sync-9.png)

¡Excelente! Ahora puede utilizar los datos de este objeto personalizado en campañas inteligentes y listas inteligentes.

>[!MORELIKETHIS]
>
>[Agregar o quitar un campo de objeto personalizado como restricciones de lista/Déclencheur inteligente](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}
