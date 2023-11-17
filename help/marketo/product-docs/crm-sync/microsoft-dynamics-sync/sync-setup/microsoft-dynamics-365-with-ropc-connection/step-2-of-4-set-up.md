---
description: 'Paso 2 de 4: Configuración de la solución Marketo con la conexión de control de contraseña del propietario de los recursos - Documentos de Marketo - Documentación del producto'
title: 'Paso 2 de 4: Configuración de la solución Marketo con la conexión de control de contraseña del propietario de los recursos'
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Paso 2 de 4: Configurar la solución de Marketo con la conexión de control de contraseña del propietario de los recursos {#step-2-of-4-set-up-the-marketo-solution-ropc}

Empecemos por crear una cuenta de usuario.

>[!PREREQUISITES]
>
>[Paso 1 de 4: Instalar la solución de Marketo con la conexión de control de contraseña del propietario de los recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Crear un nuevo usuario {#create-a-new-user}

1. Inicie sesión en Dynamics. Haga clic en el icono Settings y seleccione **[!UICONTROL Configuración avanzada]**.

   ![](assets/one.png)

1. Clic **[!UICONTROL Configuración]** y seleccione **[!UICONTROL Seguridad]**.

   ![](assets/two.png)

1. Clic **[!UICONTROL Usuarios]**.

   ![](assets/three.png)

1. Clic **[!UICONTROL Nuevo]**.

   ![](assets/four.png)

1. Clic **[!UICONTROL Agregar y autorizar usuarios]** en la nueva ventana.

   ![](assets/five.png)

1. Se abre una nueva pestaña. Clic **[!UICONTROL Administrador]** en la parte superior de la página.

   ![](assets/six.png)

1. Se abre otra pestaña nueva. Clic **[!UICONTROL Agregar un usuario]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >El usuario de sincronización debe tener permiso de lectura para la configuración de Marketo.

1. Escriba toda la información. Cuando haya terminado, haga clic en **[!UICONTROL Añadir]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Este nombre debe ser un usuario de sincronización dedicado y no una cuenta de usuario de CRM existente. No necesita ser una dirección de correo electrónico real.

1. Introduzca el correo electrónico para recibir las nuevas credenciales de usuario y haga clic en **[!UICONTROL Enviar correo electrónico y cerrar]**.

   ![](assets/nine.png)

## Asignar función de usuario de sincronización {#assign-sync-user-role}

Asigne la función Usuario de sincronización de Marketo únicamente al usuario de sincronización de Marketo. No es necesario asignarlo a ningún otro usuario.

>[!NOTE]
>
>Esto se aplica a la versión 4.0.0.14 y posteriores de Marketo. Para las versiones anteriores, todos los usuarios deben tener la función de usuario de sincronización. Para actualizar Marketo, consulte [Actualizar la solución de Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>La configuración de idioma del usuario de sincronización [debe establecerse en inglés](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Vuelva a la **[!UICONTROL Usuarios habilitados]** y actualice la lista de usuarios.

   ![](assets/ten.png)

1. Pase el ratón sobre el usuario de sincronización de Marketo que acaba de crear y aparecerá una casilla de verificación. Haga clic en para seleccionarlo.

   ![](assets/eleven.png)

1. Clic **[!UICONTROL Administrar funciones]**.

   ![](assets/twelve.png)

1. Marque **[!UICONTROL Usuario de sincronización de Marketo]** y haga clic en **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Cualquier actualización realizada en su CRM por el usuario de sincronización _no_ se sincronizarán de nuevo con Marketo.

## Configuración de la solución Marketo {#configure-marketo-solution}

¡Ya casi está! Todo lo que nos queda es informar a Marketo Solution sobre el nuevo usuario creado.

1. Vuelva a la sección Configuración avanzada y haga clic en ![](assets/image2015-5-13-15-3a49-3a19.png) junto a Configuración y seleccione **[!UICONTROL Configuración de Marketo]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si no lo ve... **[!UICONTROL Configuración de Marketo]** en el menú Configuración, actualice la página. Si eso no funciona, intente lo siguiente [publicación de la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"} o cierre la sesión y vuelva a iniciarla.

1. Clic **[!UICONTROL Predeterminado]**.

   ![](assets/fifteen.png)

1. Haga clic en el botón de búsqueda en **[!UICONTROL Usuario de Marketo]** y seleccione el usuario sync que ha creado.

   ![](assets/sixteen.png)

1. Haga clic en ![](assets/image2015-3-13-15-3a10-3a11.png) en la esquina inferior derecha para guardar los cambios.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Haga clic en **X** en la esquina superior derecha para cerrar la pantalla.

   ![](assets/seventeen.png)

1. Haga clic en ![](assets/image2015-5-13-15-3a49-3a19-1.png) junto a Configuración y seleccione **[!UICONTROL Soluciones]**.

   ![](assets/eighteen.png)

1. Haga clic en **[!UICONTROL Publicar todas las personalizaciones]** botón.

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Paso 3 de 4: Conexión de la solución Marketo con la conexión de control de contraseña del propietario de los recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
