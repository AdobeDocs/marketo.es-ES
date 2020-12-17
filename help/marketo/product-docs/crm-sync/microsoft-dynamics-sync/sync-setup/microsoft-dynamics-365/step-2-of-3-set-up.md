---
unique-page-id: 3571827
description: Paso 2 de 3 - Configuración del usuario de sincronización de marketing en Dynamics - Documentos de marketing - Documentación del producto
title: 'Paso 2 de 3: Configuración del usuario de sincronización de marketing en Dynamics'
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---


# Paso 2 de 3: Configurar usuario de sincronización de marketing en Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Comencemos creando una cuenta de usuario.

>[!PREREQUISITES]
>
>[Paso 1 de 3: Instalación de la solución de marketing (en línea)](step-1-of-3-install.md)

## Crear un nuevo usuario {#create-a-new-user}

1. Inicie sesión en Dynamics. Haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en** Configuración** y seleccione **Seguridad**.

   ![](assets/two.png)

1. Haga clic en **Usuarios**.

   ![](assets/three.png)

1. Haga clic en **Nuevo.**

   ![](assets/four.png)

1. Haga clic en **Añadir y autorizar usuarios** en la nueva ventana.

   ![](assets/five.png)

1. Se abre una nueva ficha. Haga clic en **Administración** en la parte superior de la página.

   ![](assets/six.png)

1. Se abre otra pestaña nueva. Haga clic en **Añadir un usuario**.

   ![](assets/seven.png)

1. Escriba toda la información. Cuando haya terminado, haga clic en **Añadir**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Este nombre debe ser un usuario de sincronización dedicado y no una cuenta de usuario de CRM existente. No necesita ser una dirección de correo electrónico real.

1. Introduzca el correo electrónico para recibir las credenciales de usuario nuevas y haga clic en **Enviar correo electrónico y cerrar**.

   ![](assets/nine.png)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función de usuario de sincronización de marketing solo al usuario de sincronización de marketing. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a la versión 4.0.0.14 y posterior de Marketing. Para las versiones anteriores, todos los usuarios deben tener la función de sincronización de usuarios. Para actualizar Marketing, consulte [Actualización de la solución de marketing para Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Vuelva a la ficha Usuarios habilitados y actualice la lista de usuarios.

   ![](assets/ten.png)

1. Pase el ratón por encima junto al usuario de sincronización de marketing y aparecerá una casilla de verificación. Haga clic para seleccionarlo.

   ![](assets/eleven.png)

1. Haga clic en **Administrar funciones**.

   ![](assets/twelve.png)

1. Marque **Usuario de sincronización de marketing** y haga clic en **Aceptar**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización **no** se sincronizará de nuevo con Marketing.

## Configurar la solución de marketing {#configure-marketo-solution}

¡Casi ahí! Todo lo que nos queda es informar a la solución de marketing sobre el nuevo usuario creado.

1. Vuelva a la sección Configuración avanzada y haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19.png)situado junto a Configuración y seleccione **Configuración de marketing**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si no ve **Configuración de marketing** en el menú Configuración, actualice la página. Si eso no funciona, intente [publicar de nuevo la solución de marketing](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) [](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) o cierre la sesión y vuelva a iniciarla.

1. Haga clic en **Predeterminado**.

   ![](assets/fifteen.png)

1. Haga clic en el botón de búsqueda del campo **Usuario de marketing** y seleccione el usuario de sincronización que ha creado.

   ![](assets/sixteen.png)

1. Haga clic en el icono ![](assets/image2015-3-13-15-3a10-3a11.png)en la esquina inferior derecha para guardar los cambios.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Haga clic en la **X** en la esquina superior derecha para cerrar la pantalla.

   ![](assets/seventeen.png)

1. Haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19-1.png)junto a Configuración y seleccione **Soluciones**.

   ![](assets/eighteen.png)

1. Haga clic en el botón **Publicar todas las personalizaciones**.

   ![](assets/nineteen.png)

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

    * Si desea restringir el número de registros que sincroniza, [configure un filtro de sincronización personalizado](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
    * Ejecute el proceso [Validar Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica que la configuración inicial se realizó correctamente.
    * Inicie sesión en el usuario de sincronización de marketing en Microsoft Dynamics CRM.

>[!NOTE]
>
>**Artículos relacionados**
>
>
>[Paso 3 de 3: Conectar Microsoft Dynamics con Marketing (en línea)](step-3-of-3-connect.md)
