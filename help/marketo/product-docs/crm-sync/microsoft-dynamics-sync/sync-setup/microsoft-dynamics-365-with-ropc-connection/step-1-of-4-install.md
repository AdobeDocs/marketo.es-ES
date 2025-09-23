---
description: 'Paso 1 de 4: Instalación de la solución de Marketo con la conexión de control de contraseña del propietario de los recursos - Documentos de Marketo - Documentación del producto'
title: 'Paso 1 de 4: Instalación de la solución de Marketo con la conexión de control de contraseña del propietario de los recursos'
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 1%

---

# Paso 1 de 4: Instalar la solución de Marketo con la conexión de control de contraseña del propietario de los recursos {#step-1-of-4-install-the-marketo-solution-ropc}

Para poder sincronizar [!DNL Microsoft Dynamics] 365 y Marketo, primero debe instalar la solución Marketo en [!DNL Dynamics]. Se requieren **[!DNL Dynamics]permisos de administración.**

>[!CAUTION]
>
>* No habilite la sincronización de entidades personalizada antes de completar la sincronización inicial. Se le notificará por correo electrónico una vez que se haya completado la sincronización inicial.
>* Si tienes Multi-Factor Authentication (MFA) habilitada para tu sincronización de [!DNL Dynamics], debes deshabilitarla para que [!DNL Dynamics] se sincronice correctamente con Marketo. Para obtener más información, comuníquese con [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Después de sincronizar Marketo con un CRM, no se puede realizar una nueva sincronización sin reemplazar la instancia.

>[!PREREQUISITES]
>
>[Descargar la solución Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Iniciar sesión en **[[!DNL Microsoft Office 365]](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Haga clic en el menú ![](assets/image2015-3-16-16-3a1-3a13.png) y seleccione **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Haga clic en el menú ![](assets/image2015-5-13-10-3a5-3a8.png). En el menú desplegable, seleccione **[!UICONTROL Configuración]** y, a continuación, seleccione **[!UICONTROL Soluciones]**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Haga clic en **[!UICONTROL Elegir archivo]**. Seleccione la solución Marketo Lead Management [descargada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Vea la información de la solución y haga clic en **[!UICONTROL Ver detalles del paquete de la solución]**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Cuando termine de comprobar todos los detalles, haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Ahora, en la página Información de la solución, haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Asegúrese de que la casilla de verificación de la opción SDK esté seleccionada. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Deberá habilitar las ventanas emergentes en el explorador para completar el proceso de instalación.

1. Ahora espere a que finalice la importación. Levántate y haz algunos estiramientos.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Haga clic en **[!UICONTROL Cerrar]**.

   >[!NOTE]
   >
   >Puede ver un mensaje que dice &quot;Marketo Lead Management completado con advertencia&quot;. Esto es totalmente esperado.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. &quot;Marketo Lead Management&quot; aparecerá ahora en la lista de soluciones.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Seleccione **[!UICONTROL Marketo Lead Management]** y haga clic en **[!UICONTROL Publicar todas las personalizaciones]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   ¡Buen trabajo! La instalación ha finalizado.

   >[!MORELIKETHIS]
   >
   >[Paso 2 de 4: Configurar la solución Marketo con conexión de control de contraseña de propietario de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
