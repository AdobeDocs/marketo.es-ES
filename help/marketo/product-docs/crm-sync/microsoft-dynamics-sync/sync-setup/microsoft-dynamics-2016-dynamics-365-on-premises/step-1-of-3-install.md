---
description: 'Instalar Marketo para Microsoft Dynamics 2016/Dynamics 365 local 1 de 3: documentos de Marketo: documentación del producto'
title: Instale Marketo para Microsoft Dynamics 2016/Dynamics 365 local, paso 1 de 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Paso 1 de 3: Configuración del usuario de sincronización para Marketo (2016 local/Dynamics 365 local) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Para poder sincronizar Microsoft Dynamics 2016 On-Prem/Dynamics 365 con Marketo Engage, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede sincronizar un nuevo CRM con la instancia de Marketo existente.

>[!PREREQUISITES]
>
>Si usa Microsoft Dynamics local, debe tener [Implementación con conexión a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS) configurado. Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargue Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} antes de comenzar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics**.
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en Dynamics. Haga clic en el menú desplegable **[!UICONTROL Microsoft Dynamics CRM]** y seleccione **[!UICONTROL Configuración]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. En **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Soluciones]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Haga clic en **[!UICONTROL Examinar]** y seleccione la solución que [descargó](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Haga clic en **Siguiente**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Vea la información de la solución y haga clic en **[!UICONTROL Ver detalles del paquete de la solución]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Cuando termine de comprobar todos los detalles, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/step6.png)

1. Vuelva a la página Información de la solución y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Asegúrese de que la casilla de verificación de la opción SDK esté seleccionada. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Espere a que finalice la importación.

   >[!TIP]
   >
   >Deberá habilitar las ventanas emergentes en el explorador para completar el proceso de instalación.

   ![](assets/image2015-3-11-11-34-9.png)

1. Descargue un archivo de registro (si lo desea) y haga clic en **[!UICONTROL Cerrar]**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Marketo Lead Management completado con advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management aparecerá en la página **[!UICONTROL Todas las soluciones]**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Seleccione la solución Marketo y haga clic en **[!UICONTROL Publish All Customization]**.

   ![](assets/image2015-3-19-8-41-21.png)

   ¡Choca esos cinco! La instalación ha finalizado.

   >[!CAUTION]
   >
   >Si deshabilita cualquiera de los procesos de mensajería del SDK de Marketo, se producirá un error en la instalación.

   >[!MORELIKETHIS]
   >
   >[Instalar Marketo para Dynamics 2015 local y 365 local 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"} de 2016
