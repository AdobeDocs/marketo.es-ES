---
unique-page-id: 3571830
description: 'Paso 3 de 3: Conexión de la solución Marketo con la conexión servidor a servidor - Documentos de Marketo - Documentación del producto'
title: 'Paso 3 de 3: Conexión de la solución Marketo con la conexión servidor a servidor'
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 2%

---

# Paso 3 de 3: Conexión de la solución Marketo con la conexión servidor a servidor {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

Este es el último paso de la sincronización. ¡Ya casi llegamos!

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Instalar la solución de Marketo con conexión de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}
>* [Paso 2 de 3: Configurar la solución de Marketo con conexión de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**Permisos de administración necesarios**

>[!IMPORTANT]
>
>Si va a actualizar de autenticación básica a OAuth, debe ponerse en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para obtener ayuda sobre cómo actualizar los parámetros adicionales. Al habilitar esta función, se detendrá temporalmente la sincronización hasta que se introduzcan nuevas credenciales y se vuelva a habilitar la sincronización. La función se puede deshabilitar (hasta abril de 2022) si desea volver al modo de autenticación anterior.

>[!NOTE]
>
>Antes de introducir nuevas credenciales, puede hacer lo siguiente [validarlos aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

## Introducir información de usuario de sincronización de Dynamics {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **[!UICONTROL Administrador]**.

   ![](assets/login-admin.png)

1. Clic **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Seleccionar **[!DNL Microsoft]**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Clic **[!UICONTROL Editar]** in **[!UICONTROL Introducir credenciales]**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Asegúrese de que la URL de su organización sea correcta, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se utiliza una URL de organización incorrecta, debe obtener una nueva suscripción de Marketo. Si no conoce la dirección URL, [obtenga información sobre cómo encontrarlo aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

1. Introduzca la información de usuario de Dynamics Sync y haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >El nombre de usuario en Marketo debe coincidir con el de [dirección de email](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} del usuario de la aplicación en CRM. El formato puede ser `user@domain.com` o DOMINIO\usuario.

## Seleccionar campos para sincronizar {#select-fields-to-sync}

1. Clic **[!UICONTROL Editar]** in **[!UICONTROL Seleccionar campos para sincronizar]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleccione los campos que desea sincronizar con Marketo para que se preseleccionen. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo en Dynamics, se recomienda hacerlo con la variable [sincronización deshabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Then refresh the schema in Marketo by editing and saving the [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **[!DNL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clic **[!UICONTROL Editar]** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Habilitar sincronización {#enable-sync}

1. Clic **[!UICONTROL Editar]** in **[!UICONTROL Habilitar sincronización]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de Microsoft Dynamics o cuando introduzca manualmente personas o posibles clientes.

1. Lea todo en la ventana emergente, escriba su dirección de correo electrónico y haga clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La primera sincronización puede tardar unas horas. Una vez hecho esto, recibirás una notificación por correo electrónico.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

¡Excelente trabajo!
