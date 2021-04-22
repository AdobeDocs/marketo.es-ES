---
description: Edición de campos para sincronizar antes de eliminarlos en Dynamics - Marketo Docs - Documentación del producto
title: Edición de campos para sincronizar antes de eliminarlos en Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Edición de campos para sincronizar antes de eliminarlos en Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

A veces, es posible que desee eliminar campos en Dynamics. Marketo mantiene la lista de campos como referencia para basar la sincronización en . Si se elimina un campo en Dynamics mientras la sincronización está activada, es posible que se encuentren errores en la sincronización. Antes de eliminar cualquier campo, siga los pasos a continuación.

1. En Marketo, haga clic en **Admin**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. En Integración, haga clic en **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Haga clic en **Deshabilitar sincronización**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. En una ficha nueva del explorador, inicie sesión en Dynamics y elimine los campos que desee.

1. De nuevo en Marketo, en Microsoft Dynamics, haga clic en **Editar** junto a &quot;Paso 2: Seleccione Campos para sincronizar.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Revise los campos y haga clic en **Save**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Es necesario hacer clic en **Guardar** para guardar el esquema actualizado para la sincronización, aunque no se hayan realizado cambios.

>[!NOTE]
>
>Si la sincronización no se detiene antes de eliminar un campo en Dynamics, puede que se produzcan errores en la sincronización. Si lo hace, la sincronización se detendrá. Antes de continuar, el administrador de Marketo tendría que revisar &quot;Seleccionar campos para sincronizar&quot; (descrito anteriormente) y hacer clic en **Guardar** para que la sincronización acepte los cambios de esquema.

Recuerde habilitar la sincronización después de guardar los cambios.
