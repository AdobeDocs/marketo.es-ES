---
description: Obtenga información sobre cómo editar campos para sincronizarlos en Marketo antes de eliminarlos en Dynamics. Deshabilite la sincronización, actualice el esquema y elimine el campo de la selección de sincronización.
title: Edición de campos para sincronizar antes de eliminarlos en Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/vM7JJUlegPvtRlqgPJSIjDeq9jMMUr2PA6OAC-CopJI'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 4%
---
# Edición de campos para sincronizar antes de eliminarlos en [!DNL Dynamics] {#editing-fields-to-sync-before-deleting-them-in-dynamics}

A veces es posible que desee eliminar campos en [!DNL Dynamics]. Marketo mantiene la lista de campos como referencia en la que basar la sincronización. Si se elimina un campo en [!DNL Dynamics] mientras la sincronización está activada, la sincronización podría encontrar errores. Antes de eliminar cualquier campo, siga los pasos a continuación.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. En [!UICONTROL Integración], haga clic en **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Haga clic en **[!UICONTROL Deshabilitar sincronización]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. En una nueva pestaña del explorador, inicie sesión en [!DNL Dynamics] y elimine los campos que desee.

1. En Marketo, en [!DNL Microsoft Dynamics], haga clic en **[!UICONTROL Editar]** junto a &quot;[!UICONTROL Paso 2: Seleccionar campos para sincronizar]&quot;.

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Revise los campos y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Se requiere hacer clic en **[!UICONTROL Guardar]** para guardar el esquema actualizado para la sincronización, aunque no se hayan realizado cambios.

>[!NOTE]
>
>Si la sincronización no se detiene antes de eliminar un campo en [!DNL Dynamics], la sincronización puede encontrar errores. Si es así, la sincronización se detendrá. Antes de continuar, el administrador de Marketo tendría que revisar &quot;[!UICONTROL Seleccionar campos para sincronizar]&quot; (mencionado anteriormente) y hacer clic en **[!UICONTROL Guardar]** para que la sincronización acepte los cambios de esquema.

Recuerde habilitar la sincronización después de guardar los cambios.
