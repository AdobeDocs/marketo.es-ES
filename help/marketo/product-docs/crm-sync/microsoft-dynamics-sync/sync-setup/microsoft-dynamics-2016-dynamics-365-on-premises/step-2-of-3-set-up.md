---
description: 'Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 local, paso 2 de 3: documentos de Marketo: documentación del producto'
title: Instale Marketo para Microsoft Dynamics 2016/Dynamics 365 local, paso 2 de 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Paso 2 de 3 Configuración de Marketo para Dynamics (2016 local/Dynamics 365 local){#step-of-set-up-for-marketo-on-premises-2016}

Bueno trabajo que completa los pasos anteriores. Vamos a seguir avanzando a través de esto.

>[!PREREQUISITES]
>
>[Instale Marketo para Microsoft Dynamics 2016/Dynamics 365 local, paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Crear un nuevo usuario {#create-a-new-user}

1. Inicie sesión en Dynamics. Haga clic en el icono Configuración y seleccione Configuración avanzada.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Clic **Configuración** y seleccione **Seguridad**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Clic **Usuarios**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Clic **Nuevo**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Clic **Agregar y autorizar usuarios**. Se debe abrir una nueva pestaña.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Clic **Administrador** en la parte superior de la página. Se debe abrir otra pestaña nueva.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Clic **Agregar un usuario**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Escriba toda la información. Cuando haya terminado, haga clic en **Añadir**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Este nombre debe ser un usuario de sincronización dedicado y no una cuenta de usuario de CRM existente. No necesita ser una dirección de correo electrónico real.

1. Introduzca el correo electrónico para recibir las nuevas credenciales de usuario y haga clic en Enviar correo electrónico y cerrar.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Crear una nueva aplicación cliente {#create-a-new-client-application}

Siga los pasos de [este artículo de Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) para crear una nueva aplicación cliente y conceder permisos. Tome nota del ID/secreto de cliente de la aplicación cliente de Dynamics.

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función Usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a la versión 4.0.0.14 y posteriores de Marketo. Para las versiones anteriores, todos los usuarios deben tener la función de usuario de sincronización. Para actualizar su Marketo, consulte [Actualizar la solución de Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>La configuración de idioma del usuario de sincronización [debe establecerse en inglés](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. En **Configuración**, haga clic en **Seguridad**.

   ![](assets/assign1.png)

1. Clic **Usuarios**.

   ![](assets/assign2.png)

1. Aquí verá una lista de usuarios. Seleccione al usuario de sincronización de Marketo o póngase en contacto con su [Servicios de federación de Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) para crear un usuario dedicado para Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleccione el usuario de sincronización. Clic **Administrar funciones**.

   ![](assets/assign4.png)

   Compruebe el Usuario de sincronización de Marketo y haga clic en Aceptar.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Si no ve la función, vuelva a [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizarán de nuevo con Marketo.

## Configuración de la solución Marketo {#configure-marketo-solution}

¡Ya casi terminamos! Solo tenemos unas pocas piezas de configuración antes de pasar al siguiente artículo.

1. En **Configuración**, haga clic en **Configuración de Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketo, intente actualizar la página. Si el problema persiste, [publicación de la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) o intente cerrar la sesión y volver a iniciarla.

1. Clic **Predeterminado**.

   ![](assets/configure2.png)

1. Haga clic en **Usuario de Marketo** y seleccione el usuario sync.

   ![](assets/configure3.png)

1. Haga clic en el icono de guardar en la esquina inferior derecha.

   ![](assets/configure4.png)

1. Clic **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configuración de un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
* Ejecute el [Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) proceso. Comprueba que las configuraciones iniciales se hayan realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instale Marketo para Microsoft Dynamics 2016/Dynamics 365 local, paso 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
