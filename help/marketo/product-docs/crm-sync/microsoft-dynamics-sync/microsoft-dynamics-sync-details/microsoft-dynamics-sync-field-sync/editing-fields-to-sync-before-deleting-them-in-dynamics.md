---
description: 'Edición de campos para sincronizar antes de eliminarlos en Dynamics: documentos de Marketo, documentación del producto'
title: Edición de campos para sincronizar antes de eliminarlos en Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Edición de campos para sincronizar antes de eliminarlos en Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

A veces, es posible que desee eliminar campos en Dynamics. Marketo mantiene la lista de campos como referencia en la que basar la sincronización. Si se elimina un campo en Dynamics mientras la sincronización está activada, la sincronización podría encontrar errores. Antes de eliminar cualquier campo, siga los pasos a continuación.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. En Integración, haga clic en **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Clic **Deshabilitar sincronización**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. En una nueva pestaña del explorador, inicie sesión en Dynamics y elimine los campos que desee.

1. En Marketo, en Microsoft Dynamics, haga clic en **Editar** junto a &quot;Paso 2: Seleccione los campos que desea sincronizar&quot;.

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Revise los campos y haga clic en **Guardar**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Clic **Guardar** es necesario para guardar el esquema actualizado para la sincronización, incluso si no se han realizado cambios.

>[!NOTE]
>
>Si la sincronización no se detiene antes de eliminar un campo en Dynamics, la sincronización puede encontrar errores. Si es así, la sincronización se detendrá. Antes de continuar, el administrador de Marketo tendría que revisar &quot;Seleccionar campos para sincronizar&quot; (mencionado anteriormente) y hacer clic en **Guardar** para que la sincronización acepte los cambios de esquema.

Recuerde habilitar la sincronización después de guardar los cambios.
