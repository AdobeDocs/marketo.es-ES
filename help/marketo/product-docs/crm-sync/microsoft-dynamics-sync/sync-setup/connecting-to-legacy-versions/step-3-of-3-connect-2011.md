---
unique-page-id: 3571809
description: 'Paso 3 de 3: Conexión  [!DNL Microsoft Dynamics] con Marketo (local de 2011): Documentos de Marketo: documentación del producto'
title: 'Paso 3 de 3: Conexión [!DNL Microsoft Dynamics] con Marketo (local de 2011)'
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 2%

---

# Paso 3 de 3: Conexión de [!DNL Microsoft Dynamics] con Marketo (2011 local) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

¡Bien! Instalamos la solución y configuramos el usuario de sincronización. A continuación, debemos conectar Marketo y [!DNL Dynamics].

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Instalar la solución de Marketo (local de 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)
>* [Paso 2 de 3: Configurar el usuario de sincronización de Marketo en [!DNL Dynamics] (local de 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)

>[!NOTE]
>
>**Se requieren permisos de administración**

## Escriba la información de usuario de sincronización [!DNL Dynamics] {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketo y haga clic en **[!UICONTROL Administrador]**.

   ![](assets/login-admin.png)

1. Haz clic en **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Haga clic en **[!UICONTROL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Haga clic en **[!UICONTROL Editar]** en **[!UICONTROL Paso 1: Escriba las credenciales]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales sean correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, tendrá que obtener una nueva suscripción de Marketo.

1. Escriba **[!UICONTROL Nombre de usuario]**, **[!UICONTROL Contraseña]** y **[!UICONTROL URL]** de CRM y, a continuación, haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* El [!UICONTROL nombre de usuario] de Marketo debe coincidir con el nombre de usuario del usuario de sincronización en CRM. El formato puede ser `user@domain.com` o DOMAIN\user.
   >* Si no conoce la dirección URL, [aprenda a encontrarla aquí](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## Seleccionar campos para sincronización {#select-fields-to-sync}

Ahora necesitamos seleccionar los campos sobre los que queremos sincronizar.

1. Haga clic en **[!UICONTROL Editar]** en **[!UICONTROL Paso 2: Seleccionar campos para sincronizar]**.

   ![](assets/image2015-3-16-9-51-28a.png)

1. Hay campos preseleccionados que se sincronizan. Agregue más si lo desea y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo de [!DNL Dynamics], se recomienda hacerlo con la [sincronización deshabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). A continuación, actualice el esquema en Marketo editando y guardando [Seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haz clic en **[!UICONTROL Editar]** en [!UICONTROL Detalles de sincronización de campos].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **[!UICONTROL Editar]** en **[!UICONTROL Paso 3: Habilitar sincronización]**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de [!DNL Microsoft Dynamics] ni cuando se introduzcan manualmente personas o posibles clientes.

1. Lee todo en la ventana emergente, escribe tu correo electrónico y haz clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Según el número de registros, la sincronización inicial puede tardar entre unas horas y unos días. Recibirá una notificación por correo electrónico una vez completada.

   ![](assets/image2014-12-11-11-3a55-3a15.png)
