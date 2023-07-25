---
unique-page-id: 3571813
description: 'Paso 1 de 3: Instalación de la solución de Marketo en Dynamics (local de 2013): Documentos de Marketo: documentación del producto'
title: 'Paso 1 de 3: Instalación de la solución de Marketo en Dynamics (2013 local)'
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Paso 1 de 3: Instalar la solución de Marketo en Dynamics (2013 local) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Para poder sincronizar Microsoft Dynamics local y Marketo, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>Debe tener [Implementación con Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) Configurado 2.0, 2.1 o 3.0 (ADFS). Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de empezar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Iniciar sesión en **Dynamics**. Haga clic en **Microsoft Dynamics CRM** menú desplegable y seleccione **Configuración**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. En **Configuración**, seleccione **Soluciones**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Clic **Importar**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Clic **Examinar** y seleccione la [solución descargada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clic **Siguiente**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Vea la información de la solución y haga clic en **Ver detalles del paquete de solución**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Asegúrese de que la opción SDK esté seleccionada. Clic **Importar**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Espere a que finalice la importación.

   >[!TIP]
   >
   >Deberá habilitar las ventanas emergentes en el explorador para completar el proceso de instalación.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Descargue un archivo de registro (si lo desea) y haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Marketo Lead Management completado con advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management aparecerá ahora en el **Todas las soluciones** página.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Seleccione la solución Marketo y haga clic en **Publicar todas las personalizaciones**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

No fue tan malo, ¿verdad? Vamos, voy a seguir caminando por el resto.

>[!CAUTION]
>
>Si deshabilita cualquiera de los procesos de mensajería del SDK de Marketo, se producirá un error en la instalación.

>[!MORELIKETHIS]
>
>[Paso 2 de 3: Configuración de la sincronización de usuarios con Marketo (2013 local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
