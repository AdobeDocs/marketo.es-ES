---
unique-page-id: 4719300
description: Agregar o quitar campos de objetos personalizados como restricciones de listas inteligentes o Déclencheur - Documentos de Marketo - Documentación del producto
title: Agregar o quitar campos de objetos personalizados como restricciones de listas inteligentes o Déclencheur
exl-id: 639e73eb-9a8c-4b10-8e97-892abf5c5db0
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Agregar o quitar campos de objetos personalizados como restricciones de listas inteligentes o Déclencheur {#add-remove-custom-object-field-as-smart-list-trigger-constraints}

Marketo proporciona un control preciso sobre la sincronización de objetos personalizados de Salesforce. Esto le permite seleccionar los campos disponibles como restricciones en los filtros de objeto personalizados y utilizarlos como déclencheur en campañas inteligentes.

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Clic **Administrador.**

   ![](assets/image2014-12-10-13-3a9-3a47.png)

1. Clic **Administrador** y luego **Sincronización de objetos de Salesforce.**

   ![](assets/image2015-12-11-15-3a11-3a41.png)

1. **Sincronización de objetos de Salesforce** aparece en la columna izquierda.

   ![](assets/image2015-12-11-15-3a15-3a15.png)

1. Seleccione el objeto que desea modificar.

   ![](assets/image2014-12-10-13-3a10-3a11.png)

1. Clic **Editar campos visibles**.

   >[!TIP]
   >
   >Si la variable **Editar campos visibles** el botón aparece atenuado y el objeto está actualmente en uso en una lista inteligente o campaña inteligente. Elimine todas las asociaciones para continuar.

   ![](assets/image2014-12-10-13-3a10-3a25.png)

1. Si la sincronización global está habilitada, haga clic en **Deshabilitar sincronización global**.

   ![](assets/image2014-12-10-13-3a10-3a36.png)

1. Marque las casillas junto a las restricciones de filtro/déclencheur necesarias y haga clic en **Guardar**.

   ![](assets/image2014-12-10-13-3a10-3a47.png)

   >[!NOTE]
   >
   >Todos los campos están seleccionados de forma predeterminada para que sean restricciones en los filtros.

1. Haga clic en **Campos** para confirmar los cambios.

   ![](assets/image2014-12-10-13-3a10-3a56.png)

   >[!NOTE]
   >
   >No olvide volver a activar la sincronización global.

¡Guau! Ahora las listas inteligentes y las campañas inteligentes tienen aún más poder.

>[!MORELIKETHIS]
>
>[Habilitar/Deshabilitar sincronización de objetos personalizada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-custom-object-sync.md)
