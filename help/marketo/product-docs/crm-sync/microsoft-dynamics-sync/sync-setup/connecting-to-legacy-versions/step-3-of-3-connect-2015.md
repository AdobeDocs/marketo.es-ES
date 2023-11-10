---
unique-page-id: 7504744
description: 'Instalación de Marketo para Microsoft Dynamics 2015 local, paso 3 de 3: documentos de Marketo: documentación del producto'
title: Instale Marketo para Microsoft Dynamics 2015 local, paso 3 de 3
exl-id: 054bf725-7a80-4114-8360-2d86e2e33dd7
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 1%

---

# Paso 3 de 3: Conexión de Marketo Dynamics (local de 2015) {#step-of-connect-marketo-dynamics-on-premises-2015}

>[!PREREQUISITES]
>
>* [Instale Marketo para Microsoft Dynamics 2015 local, paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}
>* [Instale Marketo para Microsoft Dynamics 2015 local, paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md){target="_blank"}

>[!NOTE]
>
>**Permisos de administración necesarios**

## Introducir información de usuario de sincronización de Dynamics {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **[!UICONTROL Administrador]**.

   ![](assets/login-admin.png)

1. Clic **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Seleccionar **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Clic **[!UICONTROL Editar]** in **[!UICONTROL Introducir credenciales]**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales sean correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, tendrá que obtener una nueva suscripción de Marketo.

1. Introduzca el **[!UICONTROL Nombre de usuario]**, **[!UICONTROL Contraseña]** a Microsoft Dynamics **[!UICONTROL URL]**, y a **Id/Secreto De Cliente**. Clic **[!UICONTROL Guardar]** cuando termine.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Si el Marketo se aprovisionó antes de octubre de 2020, el ID de cliente y el secreto son campos opcionales. De lo contrario, son obligatorios. La obtención de esta información dependerá de la versión de MSD que esté utilizando.
   >* El Nombre de usuario en Marketo debe coincidir con el Nombre de usuario para el usuario de sincronización en CRM. El formato puede ser `user@domain.com` o DOMINIO\usuario.
   >* Si no conoce la dirección URL, [obtenga información sobre cómo encontrarlo aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >¿No conoce la dirección URL? Le mostraremos cómo encontrar su [URL del servicio de organización de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"} aquí.

## Seleccionar campos para sincronizar {#select-fields-to-sync}

1. Clic **[!UICONTROL Editar]** in **[!UICONTROL Seleccionar campos para sincronizar]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Seleccione los campos que desea sincronizar con Marketo para que se preseleccionen. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo en Dynamics, se recomienda hacerlo con la variable [sincronización deshabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Then refresh the schema in Marketo by editing and saving the [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clic **[!UICONTROL Editar]** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Habilitar sincronización {#enable-sync}

1. Clic **[!UICONTROL Editar]** in **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de Microsoft Dynamics ni cuando introduzca personas manualmente.

1. Lea todo en la ventana emergente, introduzca el correo electrónico y haga clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La primera sincronización puede tardar unas horas. Una vez hecho esto, recibirá una notificación por correo electrónico.

   ![](assets/image2015-3-16-9-59-51.png)

¡Excelente trabajo!
