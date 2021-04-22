---
unique-page-id: 3571813
description: 'Paso 1 de 3: Instalación de la solución Marketo en Dynamics (2013 On-Premies) - Marketo Docs - Documentación del producto'
title: 'Paso 1 de 3: Instalación de la solución Marketo en Dynamics (local 2013)'
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Paso 1 de 3: Instale la solución Marketo en Dynamics (2013 On-Premies) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Para poder sincronizar Microsoft Dynamics On-Premies y Marketo, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no podrá realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>Debe tener configurado [Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS). Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargue Marketo ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Solution antes de comenzar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en **Dynamics**. Haga clic en el menú desplegable **Microsoft Dynamics CRM** y seleccione **Settings**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. En **Settings**, seleccione **Solutions**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Haga clic en **Import**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Haga clic en **Browse** y seleccione la [solución descargada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **Siguiente**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Vea la Información de la solución y haga clic en **Ver detalles del paquete de la solución**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Asegúrese de que la opción SDK esté seleccionada. Haga clic en **Import**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Espere a que finalice la importación.

   >[!TIP]
   >
   >Deberá activar ventanas emergentes en el navegador para completar el proceso de instalación.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Descargue un archivo de registro (si lo desea) y haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Administración de posibles clientes de Marketo completado con una advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. La Administración de posibles clientes de Marketo ahora aparecerá en la página **Todas las soluciones**.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Seleccione la solución de Marketo y haga clic en **Publicar todas las personalizaciones**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

¿No era malo, verdad? Vamos, seguiré caminando por el resto.

>[!CAUTION]
>
>Si se deshabilita cualquiera de los procesos de mensajería del SDK para Marketo, se dañará la instalación.

>[!MORELIKETHIS]
>
>[Paso 2 de 3: Configuración del usuario de sincronización para Marketo (locales de 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)
