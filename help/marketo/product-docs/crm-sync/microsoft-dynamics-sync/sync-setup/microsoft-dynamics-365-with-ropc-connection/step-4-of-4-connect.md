---
description: 'Paso 4 de 4: Conexión de la solución de Marketo con la conexión de control de contraseña del propietario de los recursos - Marketo Docs - Documentación del producto'
title: 'Paso 4 de 4: Conexión de la solución de Marketo con la conexión de control de contraseña del propietario del recurso'
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
source-git-commit: 3a52db828a9bbf01b617d6e417d078d11ea30fb7
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Paso 4 de 4: Conexión de la solución de Marketo con la conexión de control de contraseña del propietario del recurso {#step-4-of-4-connect-the-marketo-solution-ropc}

Este es el último paso de la sincronización. ¡Ya casi estás ahí!

>[!PREREQUISITES]
>
>* [Paso 1 de 4: Instalación de la solución de Marketo con la conexión de control de contraseña del propietario de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Paso 2 de 4: Configurar la solución de Marketo con la conexión de control de contraseña del propietario del recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Paso 3 de 4: Configuración de la aplicación cliente en MS Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)


>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>Si está actualizando de la autenticación básica a OAuth, puede utilizar [este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) para reconfigurar la autenticación.

## Introducir información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **Administrador**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Select **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Haga clic en **Editar** en **Paso 1: Introducir credenciales**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Asegúrese de que la URL de su organización sea correcta, ya que no podemos revertir los cambios de esquema subsiguientes después del envío. Si se utiliza una URL de organización incorrecta, deberá obtener una nueva suscripción a Marketo. Si no conoce la dirección URL, [aprenda a encontrarlo aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

   >[!NOTE]
   >
   >Antes de introducir nuevas credenciales, puede [valide aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

1. Introduzca la variable **Nombre de usuario**, **Contraseña**, Microsoft Dynamics **URL**, **ID de cliente** y **Secreto del cliente**. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >El nombre de usuario en Marketo debe coincidir con el nombre de usuario para sincronizar el usuario en CRM. El formato puede ser `user@domain.com` o DOMINIO\usuario.

## Seleccionar campos para sincronizar {#select-fields-to-sync}

1. Haga clic en **Editar** en **Paso 2: Seleccionar campos para sincronizar**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleccione los campos que desea sincronizar con Marketo, de modo que se preseleccionarán. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo en Dynamics, se recomienda hacerlo con la variable [sincronizar desactivado](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). A continuación, actualice el esquema en Marketo editando y guardando el [Seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Campos de sincronización para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **Editar** en **Paso 3: Habilitar sincronización**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente con una sincronización de Microsoft Dynamics o cuando introduzca manualmente personas o posibles clientes.

1. Lea todo en la ventana emergente, introduzca su dirección de correo electrónico y haga clic en **Iniciar sincronización**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La primera sincronización puede tardar unas horas. Una vez hecho esto, recibirá una notificación por correo electrónico.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

¡Excelente trabajo!

>[!MORELIKETHIS]
>
>[Reconfiguración del método de autenticación de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)