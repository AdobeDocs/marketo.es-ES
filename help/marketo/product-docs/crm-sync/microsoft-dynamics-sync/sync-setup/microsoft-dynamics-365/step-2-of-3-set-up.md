---
unique-page-id: 3571827
description: 'Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics - Marketo Docs - Documentación del producto'
title: 'Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics'
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---


# Paso 2 de 3: Configurar usuario de sincronización de Marketo en Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Empecemos creando una cuenta de usuario.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Instalación de la solución Marketo (en línea)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

## Crear un nuevo usuario {#create-a-new-user}

1. Inicie sesión en Dynamics. Haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en **Settings** y seleccione **Security**.

   ![](assets/two.png)

1. Haga clic en **Usuarios**.

   ![](assets/three.png)

1. Haga clic en **Nuevo.**

   ![](assets/four.png)

1. Haga clic en **Add and License Users** en la nueva ventana.

   ![](assets/five.png)

1. Se abre una nueva pestaña. Haga clic en **Admin** en la parte superior de la página.

   ![](assets/six.png)

1. Se abre otra pestaña nueva. Haga clic en **Agregar un usuario**.

   ![](assets/seven.png)

1. Escriba toda la información. Cuando haya terminado, haga clic en **Agregar**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Este nombre debe ser un usuario de sincronización dedicado y no una cuenta de usuario de CRM existente. No necesita ser una dirección de correo electrónico real.

1. Introduzca el correo electrónico para recibir las nuevas credenciales de usuario y haga clic en **Send email and close**.

   ![](assets/nine.png)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a Marketo versión 4.0.0.14 y posteriores. En versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar Marketo, consulte [Solución de actualización de Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Vuelva a la pestaña Usuarios habilitados y actualice la lista de usuarios.

   ![](assets/ten.png)

1. Pase el ratón junto al usuario de sincronización de Marketo recién creado y aparecerá una casilla de verificación. Haga clic en para seleccionarlo.

   ![](assets/eleven.png)

1. Haga clic en **Administrar funciones**.

   ![](assets/twelve.png)

1. Marketo Sync User **y haga clic en** OK **.**

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizará de nuevo con Marketo.

## Configurar la solución de Marketo {#configure-marketo-solution}

¡Casi ahí! Todo lo que nos queda es informar a la solución de Marketo sobre el nuevo usuario creado.

1. Vuelva a la sección Configuración avanzada y haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19.png) situado junto a Configuración y seleccione **Configuración de Marketo**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si no ve **Marketo Config** en el menú Configuración, actualice la página. Si eso no funciona, intente [publicar de nuevo la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) o cierre la sesión y vuelva a iniciarla.

1. Haga clic en **Default**.

   ![](assets/fifteen.png)

1. Haga clic en el botón de búsqueda del campo **Marketo User** y seleccione el usuario de sincronización que ha creado.

   ![](assets/sixteen.png)

1. Haga clic en el icono ![](assets/image2015-3-13-15-3a10-3a11.png) en la esquina inferior derecha para guardar los cambios.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Haga clic en **X** en la esquina superior derecha para cerrar la pantalla.

   ![](assets/seventeen.png)

1. Haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19-1.png) situado junto a Configuración y seleccione **Soluciones**.

   ![](assets/eighteen.png)

1. Haga clic en el botón **Publicar todas las personalizaciones**.

   ![](assets/nineteen.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

    * Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
    * Ejecute el proceso [Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Comprueba que la configuración inicial se haya realizado correctamente.
    * Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Paso 3 de 3: Conectar Microsoft Dynamics con Marketo (en línea)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
