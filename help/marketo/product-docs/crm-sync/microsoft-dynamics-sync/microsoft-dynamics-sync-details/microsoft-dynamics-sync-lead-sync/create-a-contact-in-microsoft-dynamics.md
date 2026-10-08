---
unique-page-id: 10095389
description: Obtenga información sobre cómo crear un contacto en Microsoft Dynamics desde Marketo. Utilice la acción de flujo Sincronizar persona con Microsoft en una campaña de déclencheur para crear contactos en tiempo real.
title: Crear un contacto en Microsoft Dynamics
exl-id: 66cb26c0-f383-4d1e-be22-e7f8c6b266fb
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/5q84B57P88MNhaYHluCKKCYLwOonW2xj7hAUNDOmXl8'
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
source-wordcount: '136'
ht-degree: 4%
---
# Crear un contacto en [!DNL Microsoft Dynamics] {#create-a-contact-in-microsoft-dynamics}

1. Seleccione la persona solo de Marketo Engage (el tipo de Microsoft está vacío) que desee crear como contacto en Dynamics.

   ![](assets/one.png)

1. Haga clic en **[!UICONTROL Acciones de persona]** y **[!DNL Microsoft]**, y seleccione **[!UICONTROL Sincronizar persona con Microsoft]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Sincronizar como]** y seleccione **[!UICONTROL Contacto]**. Haga clic en **[!UICONTROL Ejecutar ahora]**.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Al usar la acción de flujo &quot;[!UICONTROL Sincronizar persona con Microsoft]&quot; (solo en una campaña de Déclencheur), el posible cliente/contacto se creará en tiempo real en Dynamics.

1. Marketo convierte ese registro de posible cliente de [!DNL Dynamics] en un contacto que no está asociado a ninguna cuenta de [!DNL Dynamics].

   ![](assets/image2015-10-23-9-3a43-3a33.png)

1. Ahora, puedes seleccionar **[!UICONTROL Contacto]** cuando uses la restricción Sincronizar como en un filtro de campaña inteligente.

   ![](assets/five.png)
