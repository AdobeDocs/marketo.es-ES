---
unique-page-id: 7504744
description: Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 3 de 3 - Documentos de marketing - Documentación del producto
title: Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 3 de 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Paso 3 de 3: Connect Marketing Dynamics (2015 On-Prem y 2016 365 On-Prem) {#step-of-connect-marketo-dynamics-on-premises-and-365}

>[!PREREQUISITES]
>
>* [Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Instalación de Marketing para Dynamics 2015 On-Prem y 2016 365 On-Prem Paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Se requieren permisos de administración**

## Escriba la información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketing y haga clic en **Administración**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Seleccione **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Haga clic en **Editar** en **Paso 1: Escriba Credentials**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales son correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, tendrá que obtener una nueva suscripción de marketing.

1. Introduzca **Nombre de usuario**, **Contraseña** una dirección URL **de Microsoft Dynamics** y un **Id. de cliente** opcional. Haga clic en **Guardar** cuando termine.

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >El nombre de usuario de Marketing debe coincidir con el nombre de usuario del usuario de sincronización en CRM. El formato puede ser user@domain.com o DOMINIO\usuario.

   >[!TIP]
   >
   >¿No conoce la dirección URL? Aquí le mostraremos cómo encontrar su [URL del servicio de organización de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## Seleccionar campos para sincronizar {#select-fields-to-sync}

1. Haga clic en **Editar** en **Paso 2: Seleccione Campos para sincronizar**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Seleccione los campos que desea sincronizar con el objeto de que estén preseleccionados. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que se sincronizarán con Marketing.

1. Vaya a Administración y seleccione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en Detalles de sincronización de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **Editar** en **Paso 3: Habilite Sincronizar**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización con Microsoft Dynamics o cuando introduzca personas manualmente.

1. Lea todo en la ventana emergente, escriba su correo electrónico y haga clic en **Sincronización de Inicio**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La primera sincronización puede tardar unas horas. Una vez que haya terminado, recibirá una notificación por correo electrónico.

   ![](assets/image2015-3-16-9-59-51.png)

¡Excelente trabajo!
