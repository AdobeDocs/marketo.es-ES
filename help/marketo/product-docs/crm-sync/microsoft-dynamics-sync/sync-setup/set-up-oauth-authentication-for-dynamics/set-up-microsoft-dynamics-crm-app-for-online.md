---
description: 'Configuración de la aplicación Microsoft Dynamics CRM para en línea: Marketo Docs: documentación del producto'
title: Configuración de la aplicación Microsoft Dynamics CRM para en línea
exl-id: ec3123c9-e484-4736-9831-9559cc393bd9
source-git-commit: 8b4d86f2dd5f19abb56451403cd2638b1a852d79
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Configuración de la aplicación Microsoft Dynamics CRM para en línea {#set-up-microsoft-dynamics-crm-app-for-online}

## Configuración {#set-up}

1. Vaya a https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Siga todos los pasos. En el paso 3, introduzca un nombre de aplicación relevante (por ejemplo, &quot;Integración de Marketo&quot;). En Tipos de cuentas compatibles, seleccione Cuenta en este directorio organizativo solamente.

1. Escriba el ID de la aplicación (ClientId). Tendrá que introducirlo más adelante en Marketo.

1. Conceda el consentimiento del administrador siguiendo los pasos indicados en [este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. Genere un secreto de cliente en el Centro de administración haciendo clic en **Certificados y secretos**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-1.png)

1. Haga clic en **Nuevo secreto de cliente**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-2.png)

1. Añada una descripción del Secreto del cliente y haga clic en **Agregar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-3.png)

   >[!CAUTION]
   >
   >Asegúrese de anotar el valor Secreto del cliente (que se ve en la captura de pantalla siguiente), ya que lo necesitará más adelante. Solo se muestra una vez y no podrá recuperarlo de nuevo.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-4.png)

Marketo se autentica en Azure AD con OAuth mediante las credenciales de contraseña de propietario de recurso de tipo de concesión ( ROPC). Este escenario necesita la creación de una directiva de Descubrimiento de Dominios para la aplicación específica. Con esta directiva, Azure AD redireccionará la solicitud de autenticación al servicio de federación. Para ello, la sincronización hash de contraseña debe habilitarse en AD Connect. Para obtener más información, consulte [OAuth con ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) y [Establecer una directiva secundaria para una aplicación](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Referencias adicionales [se puede encontrar aquí](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.).

Cuando termines, es hora de **Introduzca el ID de cliente y el secreto generados por Dynamics CRM en Marketo**.

## Introduzca el ID de cliente y el secreto generados por Dynamics CRM en Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

Los siguientes pasos son aplicables a Online _y_ Versiones in situ.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-5.png)

1. Haga clic en **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-6.png)

1. Haga clic en **Desactivar sincronización**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-7.png)

1. Junto a las credenciales, haga clic en **Editar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-8.png)

1. Introduzca la variable **ID de cliente** y **Secreto del cliente** recuperó anteriormente y pulse **Guardar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-9.png)

1. Haga clic en **Validar la configuración de sincronización**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-10.png)

1. Haga clic en **Siguiente**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-11.png)

1. Debería ver todas las marcas de verificación verdes. Haga clic en **Cerrar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-12.png)

   >[!NOTE]
   >
   >Si ve una X roja entre sus marcas de verificación verdes, consulte [este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para las opciones de corrección.

1. Haga clic en **Habilitar sincronización**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-13.png)

¡Y eso es todo!
