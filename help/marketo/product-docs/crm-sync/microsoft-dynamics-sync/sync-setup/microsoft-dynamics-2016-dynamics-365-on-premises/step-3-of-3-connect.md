---
description: 'Instalar Marketo para  [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 local, paso 3 de 3: documentos de Marketo: documentación del producto'
title: Instalar Marketo para  [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 local, paso 3 de 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 3%

---

# Paso 3 de 3: Conectar Marketo [!DNL Dynamics] (2016 On Prem/[!DNL Dynamics] 365 On-Premies) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Instalar Marketo para [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 local, paso 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Instalar Marketo para [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 local, paso 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)

>[!NOTE]
>
>**Se requieren permisos de administración**

## Introducir información de usuario de sincronización de [!DNL Dynamics] {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **[!UICONTROL Administrador]**.

   ![](assets/login-admin.png)

1. Haga clic en **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Seleccione **[!DNL Microsoft]**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Haga clic en **[!UICONTROL Editar]** en **Paso 1: Escriba las credenciales**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales sean correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, tendrá que obtener una nueva suscripción de Marketo.

1. Escriba **Nombre de usuario**, **Contraseña**, [!DNL Microsoft Dynamics] **URL** y **Secreto/Id. de cliente**. Haga clic en **Guardar** cuando termine.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Si el Marketo se aprovisionó antes de octubre de 2020, el ID de cliente y el secreto son campos opcionales. De lo contrario, son obligatorios. La obtención de esta información dependerá de la versión de MSD que utilice.
   >* El Nombre de usuario en Marketo debe coincidir con el Nombre de usuario para el usuario de sincronización en CRM. El formato puede ser `user@domain.com` o DOMAIN\user.
   >* Si no conoce la dirección URL, [aprenda a encontrarla aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >¿No conoce la dirección URL? Le mostraremos cómo encontrar la [[!DNL Dynamics] URL del servicio de organización](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) aquí.

## Seleccionar campos para sincronización {#select-fields-to-sync}

1. Haga clic en **[!UICONTROL Editar]** en **[!UICONTROL Paso 2: Seleccionar campos para sincronizar]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Seleccione los campos que desea sincronizar con Marketo para que se preseleccionen. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo de [!DNL Dynamics], se recomienda hacerlo con la [sincronización deshabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). A continuación, actualice el esquema en Marketo editando y guardando [Seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **[!DNL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haz clic en **[!UICONTROL Editar]** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **[!UICONTROL Editar]** en **[!UICONTROL Paso 3: Habilitar sincronización]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de [!DNL Microsoft Dynamics] ni cuando se escriban personas manualmente.

1. Lee todo en la ventana emergente, escribe tu correo electrónico y haz clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Según el número de registros, la sincronización inicial puede tardar entre unas horas y unos días. Recibirá una notificación por correo electrónico una vez completada.

   ![](assets/image2015-3-16-9-59-51.png)
