---
unique-page-id: 3571805
description: 'Paso 1 de 3: Instalación de la solución de Marketo (local de 2011): Documentos de Marketo: documentación del producto'
title: 'Paso 1 de 3: Instalación de la solución de Marketo (local de 2011)'
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Paso 1 de 3: Instalar la solución de Marketo (local de 2011) {#step-of-install-the-marketo-solution-on-premises}

Para poder sincronizar Microsoft Dynamics local y Marketo, primero debe instalar la solución Marketo en Dynamics.

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>Debe tener [Implementación con Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) Configurado 2.0, 2.1 o 3.0 (ADFS). **Nota**: el documento IFD se descarga automáticamente al hacer clic en el vínculo.
>
>[Descargar la solución Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de empezar.

>[!NOTE]
>
>**Se requieren permisos de administración de Dynamics.**
>
>Necesita privilegios de administrador de CRM para realizar esta sincronización.

1. Iniciar sesión en **Dynamics**, seleccione **Configuración** en el menú inferior izquierdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Seleccionar **Soluciones** en el árbol.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Clic **Importar**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Clic **Examinar**. Seleccione la solución Marketo Lead Management que desee [descargado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clic **Siguiente**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Vea la información de la solución y haga clic en **Ver detalles del paquete de solución**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Vuelva a la página Información de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Asegúrese de que la casilla de verificación de la opción Mensaje del SDK esté seleccionada. Clic **Siguiente**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Deberá habilitar las ventanas emergentes en el explorador para completar el proceso de instalación.

1. Ahora espere a que finalice la importación. Levántate y haz algunos estiramientos.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Haga clic en **Cerrar**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Marketo Lead Management completado con advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management aparecerá ahora en el **Todas las soluciones** página.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Seleccione Marketo Lead Management y haga clic en **Publicar todas las personalizaciones.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

No fue tan malo, ¿verdad? Vamos, voy a seguir caminando por el resto.

>[!CAUTION]
>
>Si deshabilita cualquiera de los procesos de mensajería del SDK de Marketo, se producirá un error en la instalación.

>[!MORELIKETHIS]
>
>[Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (2011 local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)
