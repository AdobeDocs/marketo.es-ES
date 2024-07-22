---
unique-page-id: 3571827
description: 'Paso 2 de 3: Configuración de la solución Marketo con conexión de servidor a servidor - Documentos de Marketo - Documentación del producto'
title: 'Paso 2 de 3: Configuración de la solución de Marketo con conexión de servidor a servidor'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Paso 2 de 3: Configurar la solución de Marketo con conexión de servidor a servidor {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[Paso 1 de 3: instale la solución Marketo con conexión de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## Crear aplicación cliente en Azure AD {#create-client-application-in-azure-ad}

1. Vaya a [este artículo de Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Siga todos los pasos. En el paso 3, introduzca un nombre de aplicación adecuado (por ejemplo, &quot;Integración de Marketo&quot;). En Tipos de cuenta admitidos, seleccione **Cuenta solo en este directorio organizativo**.

1. Anote el ID de aplicación (ClientId) y el ID de inquilino. Tendrá que introducirlo en Marketo más adelante.

1. Conceda el consentimiento del administrador siguiendo los pasos [ de este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Genere un secreto de cliente en el Centro de administración haciendo clic en **[!UICONTROL Certificados y secretos]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. Haga clic en el botón **[!UICONTROL Nuevo secreto de cliente]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. Escriba una descripción del secreto de cliente y haga clic en **[!UICONTROL Agregar]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>Asegúrese de tomar nota del valor Secreto del cliente (que se muestra en la captura de pantalla siguiente), ya que lo necesitará más adelante. Solo se muestra una vez y no podrá recuperarla de nuevo.

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## Crear usuario de aplicación en Microsoft {#create-application-user-in-microsoft}

1. Siga los pasos del siguiente vínculo para [configurar un usuario de aplicación en Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}.

   >[!IMPORTANT]
   >
   >* Al conceder permisos al usuario de la aplicación, asegúrese de asignarlo a &quot;Función de usuario de sincronización de Marketo&quot;.
   >* Tenga en cuenta la dirección de correo electrónico del usuario de la aplicación desde la opción [ver detalles](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} en Power Platform. Esta dirección de correo electrónico se utilizará como nombre de usuario al configurar la conexión a MS Dynamics en Marketo.
   >* Cualquier actualización hecha en su CRM por el usuario de sincronización **no** se sincronizará de nuevo con Marketo.

## Azure AD Federated con AD FS local {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD to ADFS Onprem necesita la creación de una directiva de detección de dominio kerberos doméstico para la aplicación específica. Con esta directiva, Azure AD redirigirá la solicitud de autenticación al servicio de federación. La sincronización de hash de contraseña debe habilitarse en AD Connect para esto. Para obtener más información, consulte [OAuth con ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} y [Establecer una directiva de hardware para una aplicación](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Se pueden encontrar referencias adicionales [aquí](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20includes%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Configuración de la solución Marketo {#configure-marketo-solution}

¡Ya casi está! Todo lo que nos queda es informar a Marketo Solution sobre el nuevo usuario creado.

1. Vuelva a la sección Configuración avanzada, haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19.png) junto a Configuración y seleccione **[!UICONTROL Configuración de Marketo]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si no ve &quot;Configuración de Marketo&quot; en el menú Configuración, actualice la página. Si eso no funciona, intente [publicar la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} de nuevo o cierre la sesión y vuelva a iniciarla.

1. Haga clic en **[!UICONTROL Predeterminado]**.

   ![](assets/fifteen.png)

1. Haga clic en el botón de búsqueda en el campo **[!UICONTROL Usuario de Marketo]** y seleccione el usuario de sincronización que ha creado.

   ![](assets/sixteen.png)

1. Haga clic en el icono ![](assets/image2015-3-13-15-3a10-3a11.png) en la esquina inferior derecha para guardar los cambios.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Haga clic en **X** en la esquina superior derecha para cerrar la pantalla.

   ![](assets/seventeen.png)

1. Haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19-1.png) junto a Configuración y seleccione **[!UICONTROL Soluciones]**.

   ![](assets/eighteen.png)

1. Haga clic en el botón **[!UICONTROL Publish All Customization]**.

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >Si está actualizando de Autenticación básica a OAuth, puede usar [este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} para reconfigurar su autenticación.

## Antes de continuar con el paso 3 {#before-proceeding-to-step}

* Si desea restringir el número de registros que sincroniza, [configure ahora un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Ejecute el proceso [Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Comprueba que las configuraciones iniciales se hayan realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Paso 3 de 3: conectar la solución de Marketo con conexión de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md){target="_blank"}
>* [Volver a configurar el método de autenticación de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
