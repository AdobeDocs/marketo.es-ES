---
unique-page-id: 3571805
description: Paso 1 de 3 - Instalación de la solución de marketing (On-premies 2011) - Documentos de marketing - Documentación del producto
title: 'Paso 1 de 3: Instalación de la solución de marketing (On-premies 2011)'
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Paso 1 de 3: Instalación de la solución de marketing (On-premies 2011) {#step-of-install-the-marketo-solution-on-premises}

Para poder sincronizar Microsoft Dynamics On-Premises y Marketing, primero debe instalar la solución de Marketing en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketing con una CRM, no podrá realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>Debe tener [Implementación de Internet Facing](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS) configurados. **Nota**: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargue la ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) solución de administración de posibles clientes de Marketing to antes de realizar el inicio.

>[!NOTE]
>
>**Se requieren permisos de administrador de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en **Dynamics**, seleccione **Settings** en el menú inferior izquierdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Seleccione **Soluciones** en el árbol.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Haga clic en **Importar**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Haga clic en **Examinar**. Seleccione la solución Administración de posibles clientes de Marketing to que [descargó](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **Siguiente**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Vista la Información de la solución y haga clic en **Detalles del paquete de la solución de Vista**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Asegúrese de que la casilla de verificación de la opción de mensaje SDK está marcada. Haga clic en **Siguiente**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Deberá activar las ventanas emergentes en el navegador para completar el proceso de instalación.

1. Ahora espere a que finalice la importación. Levántate y haz algunas camadas.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede que vea un mensaje que dice &quot;Administración de posibles clientes con marketing completada con una advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. La Administración de posibles clientes de Marketing Cloud ahora aparecerá en la página **Todas las soluciones**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Seleccione Administración de posibles clientes de Marketing to y haga clic en **Publicar todas las personalizaciones.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

¿No era tan malo, verdad? Vamos, te seguiré caminando por el resto.

>[!CAUTION]
>
>Si se deshabilita cualquiera de los procesos de mensajería de Marketing para SDK, se producirá una instalación dañada.

>[!MORELIKETHIS]
>
>[Paso 2 de 3: Configuración del usuario de sincronización de marketing en Dynamics (On-premies 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
