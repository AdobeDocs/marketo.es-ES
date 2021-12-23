---
unique-page-id: 3571809
description: 'Paso 3 de 3: Conexión de Microsoft Dynamics con Marketo (2011 On-Premies) - Marketo Docs - Documentación del producto'
title: 'Paso 3 de 3: Conexión de Microsoft Dynamics con Marketo (local 2011)'
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Microsoft Dynamics con Marketo (local de 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

¡Bien! Hemos instalado la solución y configurado el usuario de sincronización. A continuación, es necesario conectar Marketo y Dynamics.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Instalación de la solución Marketo (local 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)
>* [Paso 2 de 3: Configuración del usuario de sincronización de Marketo en Dynamics (local de 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Se requieren permisos de administrador**

## Introducir información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **Administrador**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Haga clic en **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Haga clic en **Editar** en **Paso 1: Escriba las credenciales.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales sean correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, deberá obtener una nueva suscripción a Marketo.

1. Introduzca la variable **Nombre de usuario**, **Contraseña** y CRM **URL** a continuación, haga clic en **Guardar**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* El nombre de usuario en Marketo debe coincidir con el nombre de usuario para sincronizar el usuario en CRM. El formato puede ser `user@domain.com` o DOMINIO\usuario.
   >* Si no conoce la dirección URL, [aprenda a encontrarlo aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Seleccionar campos para sincronizar {#select-fields-to-sync}

Ahora necesitamos seleccionar los campos que queremos sincronizar.

1. Haga clic en **Editar** en **Paso 2: Seleccione Campos para sincronizar.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Hay campos preseleccionados que se sincronizarán. Añada más si lo desea y haga clic en **Guardar**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

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

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **Editar** en **Paso 3: Habilitar sincronización**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente con una sincronización de Microsoft Dynamics o cuando introduzca manualmente personas o posibles clientes.

1. Lea todo en la ventana emergente, introduzca su correo electrónico y haga clic en **Iniciar sincronización**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La primera sincronización puede tardar unas horas. Una vez finalizado, recibirá una notificación por correo electrónico.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   ¡Excelente trabajo!
