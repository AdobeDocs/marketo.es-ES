---
description: 'Paso 3 de 4: Configuración de la aplicación cliente en MS Dynamics - Marketo Docs - Documentación del producto'
title: 'Paso 3 de 4: Configuración de la aplicación cliente en MS Dynamics'
source-git-commit: 598390517dea96b0503fd9c0cdfd47bd7617b48a
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Paso 3 de 4: Configuración de la aplicación cliente en MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Paso 1 de 4: Instalación de la solución de Marketo con la conexión de control de contraseña del propietario de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Paso 2 de 4: Configurar la solución de Marketo con la conexión de control de contraseña del propietario del recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. Vaya a https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Siga todos los pasos. En el paso 3, introduzca un nombre de aplicación relevante (por ejemplo, &quot;Integración de Marketo&quot;). En Tipos de cuentas compatibles, seleccione Cuenta en este directorio organizativo solamente.

1. Escriba el ID de la aplicación (ClientId). Tendrá que introducirlo más adelante en Marketo.

1. Conceda el consentimiento del administrador siguiendo los pasos indicados en [este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. Genere un secreto de cliente en el Centro de administración haciendo clic en **Certificados y secretos**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Haga clic en **Nuevo secreto de cliente**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Añada una descripción del Secreto del cliente y haga clic en **Agregar**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Asegúrese de anotar el valor Secreto del cliente (que se ve en la captura de pantalla siguiente), ya que lo necesitará más adelante. Solo se muestra una vez y no podrá recuperarlo de nuevo.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated con AD FS On-Premim {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD to ADFS Onprem necesita la creación de una directiva de Home Domain Discovery para la aplicación específica. Con esta directiva, Azure AD redireccionará la solicitud de autenticación al servicio de federación. Para ello, la sincronización hash de contraseña debe habilitarse en AD Connect. Para obtener más información, consulte [OAuth con ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) y [Establecer una directiva secundaria para una aplicación](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Referencias adicionales [se puede encontrar aquí](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.).

## Antes de continuar con el paso 4 {#before-proceeding-to-step-4}

* Si desea restringir el número de registros que sincroniza, [configurar un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ahora.
* Ejecute el [Validar Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) proceso. Comprueba que la configuración inicial se haya realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Paso 4 de 4: Conexión de la solución de Marketo con la conexión de control de contraseña del propietario del recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md)

