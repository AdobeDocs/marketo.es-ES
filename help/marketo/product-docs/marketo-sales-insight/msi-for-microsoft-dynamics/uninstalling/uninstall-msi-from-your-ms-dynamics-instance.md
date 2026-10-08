---
unique-page-id: 37355600
description: Obtenga información sobre cómo desinstalar Marketo Sales Insight de la instancia de MS Dynamics. Elimine la solución y límpiela cuando sea necesario.
title: Desinstalar MSI de su instancia de MS [!DNL Dynamics]
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
TQID: 'https://experienceleague.adobe.com/tv5uoDyp6czOdjx3D1RDZUtoDTaaZniVF5fZDWnxPPk'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 62f69a42-2389-532a-9af6-0e08fdaa397f
    internal-label: Marketo Sales Insights
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%
---
# Desinstalar MSI de su instancia de MS [!DNL Dynamics] {#uninstall-msi-from-your-ms-dynamics-instance}

Para desinstalar MSI de la instancia de MS [!DNL Dynamics], deberá realizar los pasos en Marketo y MS [!DNL Dynamics].

>[!PREREQUISITES]
>
>[Deshabilitar MS global [!DNL Dynamics] Sync](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/one-1.png)

1. Haga clic en **[!UICONTROL Insight de ventas]**.

   ![](assets/six.png)

1. Haga clic en **[!UICONTROL Editar sincronización de campos]**.

   ![](assets/seven.png)

1. Seleccione la casilla de verificación **[!UICONTROL Deshabilitar sincronización]** y haga clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >Asegúrese de [deshabilitar la sincronización global de MS Dynamics](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) antes de deshabilitar la sincronización de campos.

   ![](assets/eight.png)

## Los siguientes pasos tienen lugar en su instancia de MS [!DNL Dynamics]: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Haga clic en **[!UICONTROL Configuración avanzada]**.

1. Haga clic en **[!UICONTROL Soluciones]**.

1. Seleccione **[!UICONTROL Marketo Sales Insight]** y haga clic en el icono Eliminar.

1. Cuando aparezca el modal Desinstalar solución, haz clic en **[!UICONTROL Aceptar]**.

   La solución MS [!DNL Dynamics] tarda aproximadamente 20 minutos en desinstalarse completamente. Sin embargo, si tiene una instancia de MS [!DNL Dynamics] grande, podría tardar un poco más.

   >[!NOTE]
   >
   >Recuerde activar la sincronización de MS global [!DNL Dynamics] una vez que desinstale MSI.
