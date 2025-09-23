---
unique-page-id: 7504736
description: 'Instalación de Marketo para Microsoft Dynamics 2015 local, paso 1 de 3: Documentos de Marketo: documentación del producto'
title: Instale Marketo para Microsoft Dynamics 2015 local, paso 1 de 3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Paso 1 de 3: Configuración de la sincronización del usuario para Marketo (2015 local) {#step-of-configure-sync-user-for-marketo-on-premises-2015}

Para poder sincronizar [!DNL Microsoft Dynamics] 2015 local con Marketo, primero debe instalar la solución Marketo en [!DNL Dynamics].

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede sincronizar un nuevo CRM con la instancia de Marketo existente.

>[!PREREQUISITES]
>
>Si usa [!DNL Microsoft Dynamics] On-Premise, debe tener [Implementación con conexión a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) configurado. Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargue Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} antes de comenzar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics**.
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en **[!DNL Dynamics].** Haz clic en el menú desplegable **[!UICONTROL Microsoft Dynamics CRM]** y selecciona **[!UICONTROL Configuración]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. En **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Soluciones]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Haga clic en **[!UICONTROL Examinar]** y seleccione la solución que [descargó](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Vea la [!UICONTROL información de la solución] y haga clic en **[!UICONTROL Ver detalles del paquete de la solución]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Cuando termine de comprobar todos los detalles, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/step6.png)

1. Vuelva a la página [!UICONTROL Información de la solución] y haga clic en **[!UICONTROL Siguiente]**.

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

1. Seleccione la solución Marketo y haga clic en **[!UICONTROL Publicar todas las personalizaciones]**.

   ![](assets/image2015-3-19-8-41-21.png)

   ¡Buen trabajo! La instalación ha finalizado.

   >[!CAUTION]
   >
   >Si deshabilita cualquiera de los procesos de mensajería de Marketo SDK, se producirá un error en la instalación.

   >[!MORELIKETHIS]
   >
   >[Instalar Marketo para [!DNL Microsoft Dynamics] 2015: paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md) local
