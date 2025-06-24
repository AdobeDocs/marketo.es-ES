---
unique-page-id: 3571805
description: 'Paso 1 de 3: Instalación de la solución de Marketo (local de 2011): Documentos de Marketo: documentación del producto'
title: 'Paso 1 de 3: Instalación de la solución de Marketo (local de 2011)'
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Paso 1 de 3: Instalar la solución de Marketo (local de 2011) {#step-of-install-the-marketo-solution-on-premises}

Para poder sincronizar Microsoft Dynamics local y Marketo Engage, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>Debe tener [Implementación con conexión a Internet](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 o 3.0 (ADFS) configurados. **Nota**: el documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargue Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} antes de comenzar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics**.
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en Dynamics y seleccione **[!UICONTROL Configuración]** en el menú inferior izquierdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Seleccione **[!UICONTROL Soluciones]** en el árbol.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Haga clic en **[!UICONTROL Examinar]**. Seleccione la solución Marketo Lead Management [descargada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Vea la información de la solución y haga clic en **[!UICONTROL Ver detalles del paquete de la solución]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Cuando termine de comprobar todos los detalles, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Vuelva a la página Información de la solución y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Asegúrese de que la casilla de verificación de la opción Mensaje de SDK esté seleccionada. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Deberá habilitar las ventanas emergentes en el explorador para completar el proceso de instalación.

1. Ahora espere a que finalice la importación. Levántate y haz algunos estiramientos.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Haga clic en **[!UICONTROL Cerrar]**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Marketo Lead Management completado con advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management aparecerá en la página **Todas las soluciones**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Seleccione Marketo Lead Management y haga clic en **[!UICONTROL Publicar todas las personalizaciones]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>Si deshabilita cualquiera de los procesos de mensajería de Marketo SDK, se producirá un error en la instalación.

>[!MORELIKETHIS]
>
>[Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (2011 local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}
