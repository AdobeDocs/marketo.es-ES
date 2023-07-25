---
description: 'Instalar Marketo para Microsoft Dynamics 2016/Dynamics 365 local 1 de 3: documentos de Marketo: documentación del producto'
title: Instale Marketo para Microsoft Dynamics 2016/Dynamics 365 local, paso 1 de 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Paso 1 de 3: Configuración del usuario de sincronización para Marketo (2016 local/Dynamics 365 local) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Para poder sincronizar Microsoft Dynamics 2016 On-Prem/Dynamics 365 con Marketo, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede sincronizar un nuevo CRM con la instancia de Marketo existente.

>[!PREREQUISITES]
>
>Si utiliza Microsoft Dynamics On-Premise, debe tener [Implementación con Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) configurado. Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargar la solución Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de empezar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Iniciar sesión en **Dynamics.** Haga clic en **Microsoft Dynamics CRM** menú desplegable y seleccione **Configuración**.

   ![](assets/image2015-3-19-8-33-29.png)

1. En **Configuración**, seleccione **Soluciones**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Clic **Importar**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Clic **Examinar** y seleccione la solución que desee [descargado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clic **Siguiente**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Vea la información de la solución y haga clic en **Ver detalles del paquete de solución**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/step6.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Asegúrese de que la casilla de verificación de la opción SDK esté seleccionada. Clic **Importar**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Espere a que finalice la importación.

   >[!TIP]
   >
   >Deberá habilitar las ventanas emergentes en el explorador para completar el proceso de instalación.

   ![](assets/image2015-3-11-11-34-9.png)

1. Descargue un archivo de registro (si lo desea) y haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Marketo Lead Management completado con advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management aparecerá ahora en el **Todas las soluciones** página.

   ![](assets/image2015-3-19-8-40-38.png)

1. Seleccione la solución Marketo y haga clic en **Publicar todas las personalizaciones**.

   ![](assets/image2015-3-19-8-41-21.png)

   ¡Choca esos cinco! La instalación ha finalizado.

   >[!CAUTION]
   >
   >Si deshabilita cualquiera de los procesos de mensajería del SDK de Marketo, se producirá un error en la instalación.

   >[!MORELIKETHIS]
   >
   >[Instale Marketo para Dynamics 2015 local y 2016 365 local, paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
