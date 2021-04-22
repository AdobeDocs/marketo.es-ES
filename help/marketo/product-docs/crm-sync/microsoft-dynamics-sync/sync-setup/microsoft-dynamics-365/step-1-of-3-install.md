---
unique-page-id: 3571822
description: 'Paso 1 de 3: Instalación de la solución de Marketo (en línea): Marketo Docs: Documentación del producto'
title: 'Paso 1 de 3: Instalación de la solución Marketo (en línea)'
exl-id: 593fc014-db38-42cc-8f9f-0dd8307751e8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Paso 1 de 3: Instale la solución de Marketo (en línea) {#step-of-install-the-marketo-solution-online}

Para poder sincronizar Microsoft Dynamics 365 y Marketo, primero debe instalar la solución Marketo en Dynamics. **Se requieren permisos de administración de Dynamics.**

>[!CAUTION]
>
>* No habilite la sincronización de entidades personalizada antes de que se complete la sincronización inicial. Una vez completada la sincronización inicial, se le notificará por correo electrónico.
>* Si tiene Multi-Factor Authentication (MFA) habilitado para Dynamics Sync, debe deshabilitarlo para que Dynamics se sincronice correctamente con Marketo. Para obtener más información, póngase en contacto con el [Soporte de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).


>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no podrá realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>[Descargar la solución de administración de posibles clientes de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Inicie sesión en **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Haga clic en el menú ![](assets/image2015-3-16-16-3a1-3a13.png) y seleccione **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Haga clic en el menú ![](assets/image2015-5-13-10-3a5-3a8.png). En el menú desplegable, seleccione **Settings** y luego seleccione **Solutions**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Haga clic en **Importar.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Haga clic en **Elegir archivo.** Seleccione la solución de administración de posibles clientes de Marketo que  [descargó](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **Siguiente**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Vea la Información de la solución y haga clic en **Ver detalles del paquete de la solución**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Cuando haya terminado de comprobar todos los detalles, haga clic en **Cerrar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Ahora, de nuevo en la página Información de la solución, haga clic en **Siguiente**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Asegúrese de que la casilla de verificación de la opción SDK esté seleccionada. Haga clic en **Import**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Deberá activar ventanas emergentes en el navegador para completar el proceso de instalación.

1. Ahora espere a que finalice la importación. Levántate y haz algunas estiramientos.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Haga clic en **Cerrar.**

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Administración de posibles clientes de Marketo completado con una advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. La Administración de posibles clientes de Marketo ahora se mostrará en la lista de soluciones.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Seleccione **Administración de posibles clientes de Marketo** y haga clic en **Publicar todas las personalizaciones.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   ¡Los cinco! La instalación ha finalizado.

   >[!MORELIKETHIS]
   >
   >[Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)
