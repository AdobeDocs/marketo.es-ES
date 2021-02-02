---
unique-page-id: 7504736
description: Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 1 de 3 - Documentos de marketing - Documentación del producto
title: Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 1 de 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Paso 1 de 3: Configurar el usuario de sincronización para el marketing (2015 en prem y 2016 365 en prem) {#step-of-configure-sync-user-for-marketo-on-premises-and-365}

Antes de sincronizar In situ Microsoft Dynamics 2015 o 2016 (Dynamics 365) con Marketing, primero debe instalar la solución de Marketing en Dynamics.

>[!NOTE]
>
>Una vez que haya sincronizado Marketing con una CRM, no podrá sincronizar una nueva CRM con la instancia de Marketing existente.

>[!PREREQUISITES]
>
>Si utiliza Microsoft Dynamics On-Premise, debe tener [Implementación de Internet Facing](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) configurados. Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargue la ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) solución de administración de posibles clientes de Marketing to antes de realizar el inicio.

>[!NOTE]
>
>**Se requieren permisos de administrador de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en **Dynamics.** Haga clic en el menú desplegable  **Microsoft Dynamics** CRM y seleccione  **Configuración**.

   ![](assets/image2015-3-19-8-33-29.png)

1. En **Configuración**, seleccione **Soluciones**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Haga clic en **Importar**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Haga clic en **Examinar** y seleccione la solución que [descargó](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **Siguiente**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Vista la Información de la solución y haga clic en **Detalles del paquete de la solución de Vista**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/step6.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Asegúrese de que la casilla de verificación de la opción SDK está seleccionada. Haga clic en **Importar**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Espere a que finalice la importación.

   >[!TIP]
   >
   >Deberá activar las ventanas emergentes en el navegador para completar el proceso de instalación.

   ![](assets/image2015-3-11-11-34-9.png)

1. Descargue un archivo de registro (si lo desea) y haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede que vea un mensaje que dice &quot;Administración de posibles clientes con marketing completada con una advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-3-13-9-54-39.png)

1. La Administración de posibles clientes de Marketing Cloud ahora aparecerá en la página **Todas las soluciones**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Seleccione la solución de marketing y haga clic en **Publicar todas las personalizaciones**.

   ![](assets/image2015-3-19-8-41-21.png)

   ¡Los cinco mejores! La instalación ha finalizado.

   >[!CAUTION]
   >
   >Si se deshabilita cualquiera de los procesos de mensajería de Marketing para SDK, se producirá una instalación dañada.

   >[!MORELIKETHIS]
   >
   >[Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
