---
unique-page-id: 3571805
description: 'Paso 1 de 3: Instalación de la solución de Marketo (local de 2011): Documentos de Marketo: documentación del producto'
title: 'Paso 1 de 3: Instalación de la solución de Marketo (local de 2011)'
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 2%

---

# Paso 1 de 3: Instalar la solución de Marketo (local de 2011) {#step-of-install-the-marketo-solution-on-premises}

Para poder sincronizar el Marketo Engage y las instalaciones locales de Microsoft Dynamics, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>Debe tener [Implementación con Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} Configurado 2.0, 2.1 o 3.0 (ADFS). **Nota**: el documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargar la solución Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} antes de empezar.

>[!NOTE]
>
>**Permisos de administración de Dynamics requeridos**.
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en Dynamics y seleccione **[!UICONTROL Configuración]** en el menú inferior izquierdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Seleccionar **[!UICONTROL Soluciones]** en el árbol.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Clic **[!UICONTROL Importar]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Clic **[!UICONTROL Examinar]**. Seleccione la solución Marketo Lead Management que desee [descargado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Vea la información de la solución y haga clic en **[!UICONTROL Ver detalles del paquete de solución]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Vuelva a la página Información de la solución y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Asegúrese de que la casilla de verificación de la opción Mensaje del SDK esté seleccionada. Haga clic en **[!UICONTROL Siguiente]**.

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

1. Marketo Lead Management aparecerá ahora en el **Todas las soluciones** página.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Seleccione Marketo Lead Management y haga clic en **[!UICONTROL Publicar todas las personalizaciones]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>Si deshabilita cualquiera de los procesos de mensajería del SDK de Marketo, se producirá un error en la instalación.

>[!MORELIKETHIS]
>
>[Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (2011 local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}
