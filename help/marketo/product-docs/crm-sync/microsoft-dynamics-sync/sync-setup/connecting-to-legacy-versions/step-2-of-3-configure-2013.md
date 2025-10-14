---
unique-page-id: 3571816
description: 'Paso 2 de 3: Configuración del usuario de sincronización para Marketo (2013 local): Documentos de Marketo: documentación del producto'
title: 'Paso 2 de 3: Configuración de la sincronización del usuario para Marketo (2013 local)'
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 3%

---

# Paso 2 de 3: Configuración de la sincronización de usuarios con Marketo (2013, local) {#step-of-configure-sync-user-for-marketo-on-premises}

Buen trabajo completando los pasos anteriores, sigamos con esto.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Instalar la solución de Marketo en [!DNL Dynamics] (2013 local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función Usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a la versión del complemento de Marketo 4.0.0.14 y posterior. Para las versiones anteriores, todos los usuarios deben tener la función de usuario de sincronización. Para actualizar Marketo, consulte [Actualizar la solución Marketo para [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>La configuración de idioma del usuario de sincronización [&#x200B; debe establecerse en inglés](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Administración]**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Seleccione **[!UICONTROL Usuarios]**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Aquí verá una lista de usuarios. Seleccione al usuario de sincronización de Marketo o póngase en contacto con el administrador de [Servicios de federación de Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} para crear un nuevo usuario [dedicado a Marketo](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx){target="_blank"}.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Haga clic en ![](assets/image2015-3-26-11-3a16-3a22.png) y seleccione **[!UICONTROL Administrar roles]**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Comprueba **[!UICONTROL el usuario de sincronización de Marketo]** y haz clic en **[!UICONTROL Aceptar]**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Si no ve la función, vuelva al [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"} e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización hecha en su CRM por el usuario de sincronización _no_ se sincronizará de nuevo con Marketo.

## Configuración de la solución Marketo {#configure-marketo-solution}

¡Ya casi terminamos! Solo tenemos unas pocas piezas de configuración antes de pasar al siguiente artículo.

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Configuración de Marketo]**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Si falta la configuración de **[!UICONTROL Marketo]**, intente actualizar la página. Si el problema persiste, [vuelva a publicar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md) o intente cerrar la sesión y volver a iniciarla.

1. Haga clic en **[!UICONTROL Predeterminado]**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Haga clic en el campo **[!UICONTROL Usuario de Marketo]** y seleccione el usuario de sincronización.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Haga clic en ![](assets/image2015-3-13-15-3a10-3a11.png) en la esquina inferior derecha para guardar los cambios.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Haga clic en **[!UICONTROL Publicar todas las personalizaciones]**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configure ahora un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Ejecute el proceso [Validar [!DNL Microsoft Dynamics] Sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Comprueba que las configuraciones iniciales se hayan realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en [!DNL Microsoft Dynamics] CRM.

¡Buen trabajo!

>[!MORELIKETHIS]
>
>[Paso 3 de 3: conectar Marketo y [!DNL Dynamics] (2013 local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2013.md)
