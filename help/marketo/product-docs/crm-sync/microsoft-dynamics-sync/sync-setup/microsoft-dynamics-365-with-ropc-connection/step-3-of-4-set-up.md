---
description: 'Paso 3 de 4: Configuración de la aplicación cliente en MS Dynamics - Documentos de Marketo - Documentación del producto'
title: 'Paso 3 de 4: Configuración de la aplicación cliente en MS Dynamics'
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Paso 3 de 4: Configurar la aplicación cliente en MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Paso 1 de 4: Instalar la solución de Marketo con la conexión de control de contraseña del propietario de los recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Paso 2 de 4: Configurar la solución de Marketo con la conexión de control de contraseña del propietario de los recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Navegar a esto [Artículo de Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Siga todos los pasos. En el paso 3, introduzca un nombre de aplicación adecuado (por ejemplo, &quot;Integración de Marketo&quot;). En Tipos de cuenta admitidos, seleccione Cuenta solo en este directorio organizativo.

1. Anote el ID de la aplicación (ClientId). Tendrá que introducirlo en Marketo más adelante.

1. Conceda el consentimiento del administrador siguiendo los pasos indicados en [este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Genere un Secreto de cliente en el Centro de administración haciendo clic en **[!UICONTROL Certificados y secretos]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Clic **[!UICONTROL Nuevo secreto de cliente]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Añada una descripción del Secreto del cliente y haga clic en **[!UICONTROL Añadir]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Asegúrese de tomar nota del valor Secreto del cliente (que se muestra en la captura de pantalla siguiente), ya que lo necesitará más adelante. Solo se muestra una vez y no podrá recuperarla de nuevo.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated con AD FS local {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD to ADFS Onprem necesita la creación de una directiva de detección de dominio kerberos doméstico para la aplicación específica. Con esta directiva, Azure AD redirigirá la solicitud de autenticación al servicio de federación. La sincronización de hash de contraseña debe habilitarse en AD Connect para esto. Para obtener más información, consulte [OAuth con ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Referencias adicionales [se puede encontrar aquí](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20includes%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Antes de continuar con el paso 4 {#before-proceeding-to-step-4}

* Si desea restringir el número de registros que sincroniza, [configuración de un filtro de sincronización personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} ahora.
* Ejecute el [Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} proceso. Comprueba que las configuraciones iniciales se hayan realizado correctamente.
* Inicie sesión en el usuario de sincronización de Marketo en Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Paso 4 de 4: Conectar la solución de Marketo con la conexión de control de contraseña del propietario de los recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
