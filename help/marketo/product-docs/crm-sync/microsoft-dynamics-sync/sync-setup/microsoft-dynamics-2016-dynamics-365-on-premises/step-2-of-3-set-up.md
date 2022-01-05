---
description: Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 2 de 3 - Marketo Docs - Documentación del producto
title: Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 2 de 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Paso 2 de 3 Configuración de Marketo para Dynamics (2016 local/Dynamics 365 On-Premies){#step-of-set-up-for-marketo-on-premises-2016}

Bueno trabajo completando los pasos anteriores. Sigamos adelante.

>[!PREREQUISITES]
>
>[Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Crear un nuevo usuario {#create-a-new-user}

1. Inicie sesión en Dynamics. Haga clic en el icono Configuración y seleccione Configuración avanzada.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Haga clic en **Configuración** y seleccione **Seguridad**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Haga clic en **Usuarios**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Haga clic en **Nuevo**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Haga clic en **Agregar y conceder licencias a usuarios**. Se debe abrir una nueva pestaña.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Haga clic en **Administrador** en la parte superior de la página. Se debe abrir otra pestaña nueva.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Haga clic en **Agregar un usuario**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Escriba toda la información. Cuando haya terminado, haga clic en **Agregar**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Este nombre debe ser un usuario de sincronización dedicado y no una cuenta de usuario de CRM existente. No necesita ser una dirección de correo electrónico real.

1. Introduzca el correo electrónico para recibir las nuevas credenciales de usuario y haga clic en Enviar correo electrónico y cierre.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Crear una nueva aplicación cliente {#create-a-new-client-application}

Siga los pasos indicados en [este artículo de Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) para crear una nueva aplicación cliente y conceder permisos. Tenga en cuenta el ID de cliente/Secreto de la aplicación cliente de Dynamics.

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a Marketo versión 4.0.0.14 y posteriores. En versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar su Marketo, consulte [Actualización de la solución Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>La configuración de idioma del usuario de sincronización [debe establecerse en inglés](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. En **Configuración**, haga clic en **Seguridad**.

   ![](assets/assign1.png)

1. Haga clic en **Usuarios**.

   ![](assets/assign2.png)

1. Aquí puede ver una lista de usuarios. Seleccione el usuario de sincronización de Marketo o póngase en contacto con su [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) para crear un usuario dedicado para Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Haga clic en **Administrar funciones**.

   ![](assets/assign4.png)

   Compruebe el usuario de Marketo Sync y haga clic en Aceptar.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Si no ve la función , vuelva a [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **not** se sincronizan de nuevo con Marketo.

## Configurar la solución Marketo {#configure-marketo-solution}

¡Casi terminado! Solo tenemos algunos últimos fragmentos de configuración antes de pasar al siguiente artículo.

1. En **Configuración**, haga clic en **Configuración de Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketo, intente actualizar la página. Si el problema persiste, [publicar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) o intente cerrar la sesión y volver a iniciarla.

1. Haga clic en **Predeterminado**.

   ![](assets/configure2.png)

1. Haga clic en el **Usuario de Marketo** y seleccione el usuario de sincronización.

   ![](assets/configure3.png)

1. Haga clic en el icono Guardar en la esquina inferior derecha.

   ![](assets/configure4.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configurar un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
* Ejecute el [Validar Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) proceso. Comprueba que la configuración inicial se haya realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
