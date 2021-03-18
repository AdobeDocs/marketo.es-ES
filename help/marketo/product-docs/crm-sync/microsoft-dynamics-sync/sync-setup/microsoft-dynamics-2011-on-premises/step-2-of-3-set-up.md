---
unique-page-id: 3571807
description: 'Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (2011 On-Premies) - Marketo Docs - Documentación del producto'
title: 'Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (local de 2011)'
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# Paso 2 de 3: Configurar usuario de sincronización de Marketo en Dynamics (2011 On-Premies) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Bueno trabajo completando los pasos anteriores, sigamos adelante con esto.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Instalación de la solución Marketo (local 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica al complemento Marketo versión 4.0.0.14 y posteriores. En versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar Marketo, consulte [Actualización de la solución Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. En el menú inferior izquierdo, seleccione **Settings**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. En el árbol, seleccione **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Seleccione **Users**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Aquí puede ver una lista de usuarios. Seleccione el usuario de sincronización de Marketo dedicado o póngase en contacto con su administrador de [Servicios de federación de Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) para crear un nuevo usuario dedicado a Marketo. Haga clic en **Administrar funciones**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Marketo Sync User **y haga clic en** OK **.**

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si no ve la función , vuelva al [paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) e importe la solución.

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizará de nuevo con Marketo.

## Configurar la solución de Marketo {#configure-marketo-solution}

¡Casi terminado! Solo tenemos algunos últimos fragmentos de configuración antes de pasar al siguiente artículo.

1. Seleccione **Settings**. A continuación, seleccione **Marketo Config** en el árbol.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si falta la configuración de Marketo, intente actualizar la página. Si el problema persiste, [vuelva a publicar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) o cierre la sesión y vuelva a iniciarla.

1. Haga clic en **Default**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Haga clic en ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. En la ventana emergente, seleccione el usuario de sincronización. A continuación, haga clic en **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Haga clic en **Guardar** para guardar los cambios.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/publish-all-customizations1.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

    * Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
    * Ejecute el proceso [Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Comprueba que la configuración inicial se haya realizado correctamente.
    * Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

¡bueno trabajo!

>[!MORELIKETHIS]
>
>[Paso 3 de 3: Conectar Microsoft Dynamics con Marketo (local de 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
