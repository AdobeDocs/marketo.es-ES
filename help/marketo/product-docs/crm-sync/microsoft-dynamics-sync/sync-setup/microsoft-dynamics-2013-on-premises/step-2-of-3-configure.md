---
unique-page-id: 3571816
description: Paso 2 de 3 - Configuración del usuario de sincronización para el marketing (On-premies 2013) - Documentos de marketing - Documentación del producto
title: 'Paso 2 de 3: Configuración del usuario de sincronización para el marketing (On-premies 2013)'
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Paso 2 de 3: Configurar la sincronización de usuarios para el marketing (locales de 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Bueno trabajo al completar los pasos anteriores, sigamos avanzando.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Instalación de la solución de marketing en Dynamics (On-situ 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de marketing solo al usuario de sincronización de marketing. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica al complemento de marketing versión 4.0.0.14 y posterior. Para las versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar Marketing, consulte [Actualización de la solución de marketing para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. En **Configuración**, haga clic en **Administración**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Seleccione **Usuarios**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Aquí verá una lista de usuarios. Seleccione el usuario dedicado de Marketingto Sync o póngase en contacto con el [administrador de Servicios de federación de Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [para crear un nuevo usuario dedicado a Marketing.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Haga clic en ![](assets/image2015-3-26-11-3a16-3a22.png) y seleccione **Administrar funciones**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Marque **Usuario de sincronización de marketing** y haga clic en **Aceptar**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Si no ve la función, vuelva al [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizará de nuevo con Marketing.

## Configurar la solución de marketing {#configure-marketo-solution}

¡Casi terminado! Solo tenemos algunas últimas piezas de configuración antes de pasar al siguiente artículo.

1. En **Configuración**, haga clic en **Configuración de marketing**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Si falta **Configuración de marketing**, intente actualizar la página. Si el problema persiste, [vuelva a publicar la solución de MarketingTo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) o intente cerrar la sesión y volver a iniciarla.

1. Haga clic en **Predeterminado**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Haga clic en el campo **Usuario de marketing** y seleccione el usuario de sincronización.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Haga clic ![](assets/image2015-3-13-15-3a10-3a11.png) en la esquina inferior derecha para guardar los cambios.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
* Ejecute el proceso [Validar Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica que la configuración inicial se realizó correctamente.
* Inicie sesión en el usuario de sincronización de marketing en Microsoft Dynamics CRM.

¡bueno trabajo!

>[!MORELIKETHIS]
>
>[Paso 3 de 3: Connect Marketing y Dynamics (locales de 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
