---
unique-page-id: 3571816
description: 'Paso 2 de 3: Configuración del usuario de sincronización para Marketo (On-Premies 2013) - Documentos de Marketo: Documentación del producto'
title: 'Paso 2 de 3: Configuración del usuario de sincronización para Marketo (local 2013)'
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Paso 2 de 3: Configuración del usuario de sincronización para Marketo (On-Premies 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Bueno trabajo completando los pasos anteriores, sigamos adelante con esto.

>[!PREREQUISITES]
[Paso 1 de 3: Instalación de la solución de Marketo en Dynamics (local 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)>
>

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
Esto se aplica al complemento de Marketo versión 4.0.0.14 y posteriores. En versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar Marketo, consulte [Actualización de la solución de Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
La configuración de idioma del usuario de sincronización [debe establecerse en inglés](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. En **Configuración**, haga clic en **Administración**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Seleccione **Users**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Aquí puede ver una lista de usuarios. Seleccione su usuario de sincronización de Marketo o póngase en contacto con su administrador de [Servicios de federación de Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [para crear un nuevo usuario dedicado a Marketo.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Haga clic en ![](assets/image2015-3-26-11-3a16-3a22.png) y seleccione **Administrar funciones**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Marque **Marketo Sync User** y haga clic en **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   Si no ve la función , vuelva al [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizará de nuevo con Marketo.

## Configurar la solución de Marketo {#configure-marketo-solution}

¡Casi terminado! Solo tenemos algunos últimos fragmentos de configuración antes de pasar al siguiente artículo.

1. En **Configuración**, haga clic en **Configuración de Marketo**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   Si falta **Configuración de Marketo**, intente actualizar la página. Si el problema persiste, [vuelva a publicar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) o intente cerrar la sesión y volver a iniciarla.

1. Haga clic en **Default**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Haga clic en el campo **Marketo User** y seleccione el usuario de sincronización.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Haga clic ![](assets/image2015-3-13-15-3a10-3a11.png) en la esquina inferior derecha para guardar los cambios.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
* Ejecute el proceso [Validate Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Comprueba que la configuración inicial se haya realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

¡bueno trabajo!

>[!MORELIKETHIS]
[Paso 3 de 3: Conectar Marketo y Dynamics (local de 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
