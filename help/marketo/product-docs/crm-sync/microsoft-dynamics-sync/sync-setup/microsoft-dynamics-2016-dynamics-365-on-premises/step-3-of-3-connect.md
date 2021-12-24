---
description: Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 3 de 3 - Marketo Docs - Documentación del producto
title: Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 3 de 3
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo Dynamics (2016 En Prem/Dynamics 365 On-Premies) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Instalación de Marketo para Microsoft Dynamics 2016/Dynamics 365 On-Premies Paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Se requieren permisos de administrador**

## Introducir información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **Administrador**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Select **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Haga clic en **Editar** en **Paso 1: Introducir credenciales**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales sean correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, deberá obtener una nueva suscripción a Marketo.

1. Introduzca la variable **Nombre de usuario**, **Contraseña** a Microsoft Dynamics **URL** y **Id. de cliente/Secreto**. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Si Marketo se aprovisionó antes de octubre de 2020, el ID de cliente y Secreto son campos opcionales. De lo contrario, son obligatorios. La obtención de esta información dependerá de la versión de MSD que utilice.
   >* El nombre de usuario en Marketo debe coincidir con el nombre de usuario para sincronizar el usuario en CRM. El formato puede ser `user@domain.com` o DOMINIO\usuario.
   >* Si no conoce la dirección URL, [aprenda a encontrarlo aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


   >[!TIP]
   >
   >¿No conoces la URL? Le mostraremos cómo encontrar su [URL del servicio de organización de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) aquí.

## Seleccionar campos para sincronizar {#select-fields-to-sync}

1. Haga clic en **Editar** en **Paso 2: Seleccionar campos para sincronizar**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Seleccione los campos que desea sincronizar con Marketo, de modo que se preseleccionarán. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

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

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **Editar** en **Paso 3: Habilitar sincronización**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente con una sincronización de Microsoft Dynamics o cuando introduzca personas manualmente.

1. Lea todo en la ventana emergente, introduzca su correo electrónico y haga clic en **Iniciar sincronización**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La primera sincronización puede tardar unas horas. Una vez finalizado, recibirá una notificación por correo electrónico.

   ![](assets/image2015-3-16-9-59-51.png)

¡Excelente trabajo!
