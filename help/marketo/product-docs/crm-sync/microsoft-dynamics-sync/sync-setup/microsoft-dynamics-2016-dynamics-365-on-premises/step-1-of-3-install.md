---
description: Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies 1 de 3 - Marketo Docs - Documentación del producto
title: Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 1 de 3
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Paso 1 de 3: Configuración del usuario de sincronización para Marketo (2016 On-Premim/Dynamics 365 On-Premies) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Para poder sincronizar Microsoft Dynamics 2015 On-Premies o 2016 (Dynamics 365) con Marketo, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no podrá sincronizar un nuevo CRM con la instancia de Marketo existente.

>[!PREREQUISITES]
>
>Si utiliza Microsoft Dynamics On-Premise, debe tener [Implementación de Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) Más de 2.0 (ADFS) configurado. Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargar la solución de administración de posibles clientes de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de comenzar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Iniciar sesión en **Dinámica.** Haga clic en el **Microsoft Dynamics CRM** menú desplegable y seleccione **Configuración**.

   ![](assets/image2015-3-19-8-33-29.png)

1. En **Configuración**, seleccione **Soluciones**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Haga clic en **Importar**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Haga clic en **Examinar** y seleccione la solución [descargado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **Siguiente**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Consulte la información de la solución y haga clic en **Ver detalles del paquete de soluciones**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/step6.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Asegúrese de que la casilla de verificación de la opción SDK esté seleccionada. Haga clic en **Importar**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Espere a que finalice la importación.

   >[!TIP]
   >
   >Deberá activar ventanas emergentes en el navegador para completar el proceso de instalación.

   ![](assets/image2015-3-11-11-34-9.png)

1. Descargue un archivo de registro (si lo desea) y haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Administración de posibles clientes de Marketo completada con una advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-3-13-9-54-39.png)

1. La Administración de posibles clientes de Marketo ahora aparecerá en el **Todas las soluciones** página.

   ![](assets/image2015-3-19-8-40-38.png)

1. Seleccione la solución de Marketo y haga clic en **Publicar todas las personalizaciones**.

   ![](assets/image2015-3-19-8-41-21.png)

   ¡Los cinco! La instalación ha finalizado.

   >[!CAUTION]
   >
   >Si se deshabilita cualquiera de los procesos de mensajería del SDK para Marketo, se dañará la instalación.

   >[!MORELIKETHIS]
   >
   >[Instalación de Marketo para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
