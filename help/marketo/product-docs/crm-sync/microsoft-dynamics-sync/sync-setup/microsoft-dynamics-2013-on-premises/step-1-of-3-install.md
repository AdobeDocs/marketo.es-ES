---
unique-page-id: 3571813
description: 'Paso 1 de 3: Instalación de la solución de marketing en Dynamics (On-premies 2013) - Documentos de marketing - Documentación del producto'
title: 'Paso 1 de 3: Instalación de la solución de marketing en Dynamics (On-premies 2013)'
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Paso 1 de 3: Instalación de la solución de marketing en Dynamics (On-premies 2013) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Para poder sincronizar Microsoft Dynamics On-Premises y Marketing, primero debe instalar la solución de Marketing en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketing con una CRM, no podrá realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>Debe tener [Implementación de Internet Facing](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS) configurados. Nota: El documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargue la ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) solución de marketing antes de realizar el inicio.

>[!NOTE]
>
>**Se requieren permisos de administrador de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Inicie sesión en **Dynamics**. Haga clic en el menú desplegable **Microsoft Dynamics CRM** y seleccione **CONFIGURACIÓN**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. En **CONFIGURACIÓN**, seleccione **SOLUCIONES**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Haga clic en **Importar**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Haga clic en **Examinar** y seleccione la [solución descargada](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **Siguiente**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Vista la Información de la solución y haga clic en **Detalles del paquete de la solución de Vista**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Asegúrese de que la opción SDK está marcada. Haga clic en **Importar**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Espere a que finalice la importación.

   >[!TIP]
   >
   >Deberá activar las ventanas emergentes en el navegador para completar el proceso de instalación.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Descargue un archivo de registro (si lo desea) y haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede que vea un mensaje que dice &quot;Administración de posibles clientes con marketing completada con una advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. La Administración de posibles clientes de Marketing Cloud ahora aparecerá en la página **Todas las soluciones**.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Seleccione la solución de marketing y haga clic en **Publicar todas las personalizaciones**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

¿No era tan malo, verdad? Vamos, te seguiré caminando por el resto.

>[!CAUTION]
>
>Si se deshabilita cualquiera de los procesos de mensajería de Marketing para SDK, se producirá una instalación dañada.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Paso 2 de 3: Configuración del usuario de sincronización para Marketing (On-situ en 2013)](step-2-of-3-configure.md)

>



