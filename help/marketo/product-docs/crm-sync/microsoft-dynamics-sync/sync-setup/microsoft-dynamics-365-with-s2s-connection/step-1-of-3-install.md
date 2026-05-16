---
description: Obtenga información sobre cómo instalar la solución de Marketo en Dynamics 365 con conexión de servidor a servidor. Importe la solución desde el administrador y complete los pasos de instalación.
title: 'Paso 1 de 3: Instalación de la solución de Marketo con conexión de servidor a servidor'
exl-id: bf6f87c1-5ba5-490b-bcce-365120af3730
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/Zxz0uXhcLankhjuBt-n5T-kAuPxiSR--Jka2uybXqi4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 1%

---

# Paso 1 de 3: Instalar la solución de Marketo con conexión de servidor a servidor {#step-1-of-3-install-the-marketo-solution-s2s}

Para poder sincronizar [!DNL Microsoft Dynamics 365] y Marketo, primero debe instalar la solución de Marketo en [!DNL Dynamics]. **[!DNL Dynamics]Se requieren permisos de administrador.**

>[!CAUTION]
>
>No habilite la sincronización de entidades personalizada antes de completar la sincronización inicial. Se le notificará por correo electrónico una vez que se haya completado la sincronización inicial.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>[Descargar la solución Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}

1. Iniciar sesión en **[[!DNL Microsoft Office 365]](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Haga clic en el menú ![](assets/image2015-3-16-16-3a1-3a13.png) y seleccione **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Haga clic en el menú ![](assets/image2015-5-13-10-3a5-3a8.png). En el menú desplegable, seleccione **[!UICONTROL Configuración]** y, a continuación, seleccione **[!UICONTROL Soluciones]**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Haga clic en **[!UICONTROL Elegir archivo]**. Seleccione la solución Marketo Lead Management [descargada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **[!UICONTROL Next]**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Vea la información de la solución y haga clic en **[!UICONTROL Ver detalles del paquete de la solución]**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Cuando termine de comprobar todos los detalles, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Ahora, en la página [!UICONTROL Información de la solución], haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Asegúrese de que la casilla de verificación de la opción SDK esté seleccionada. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Deberá habilitar las ventanas emergentes en el explorador para completar el proceso de instalación.

1. Ahora espere a que finalice la importación.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Haga clic en **[!UICONTROL Cerrar]**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Marketo Lead Management completado con advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. [!UICONTROL Marketo Lead Management] aparecerá en la lista de soluciones.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Seleccione **[!UICONTROL Marketo Lead Management]** y haga clic en **[!UICONTROL Publicar todas las personalizaciones]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   La instalación ha finalizado.

   >[!MORELIKETHIS]
   >
   >[Paso 2 de 3: Configurar la solución de Marketo con conexión S2S](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
