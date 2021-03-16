---
description: Configuración de la aplicación Microsoft Dynamics CRM para On-Premim - Marketo Docs - Documentación del producto
title: Configuración de la aplicación Microsoft Dynamics CRM para On-Premim
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# Configurar la aplicación Microsoft Dynamics CRM para On-Premim {#set-up-microsoft-dynamics-crm-app-for-on-prem}

La configuración de Marketo basada en el Secreto del cliente/ID del cliente se puede realizar para On-Premim con AD FS (ver. 2016 o posterior). Para versiones anteriores de On-Premim, póngase en contacto con [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para que el método de autenticación cambie para que se base solamente en el ID de usuario y la contraseña.

## Configurar la aplicación Microsoft Dynamics CRM {#set-up-microsoft-dynamics-crm-app}

Siga los pasos de [este artículo de Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later).

Cuando haya terminado, el siguiente paso es **Introducir el Secreto e ID de cliente generado por Dynamics CRM en Marketo**.

## Introduzca el Id. de cliente generado y el secreto de Dynamics CRM en Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

Los siguientes pasos son aplicables a las versiones en línea y locales.

1. En Marketo, haga clic en **Admin**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. Haga clic en **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. Haga clic en **Deshabilitar sincronización**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. Junto a las credenciales, haga clic en **Editar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. Introduzca el **Client Id** y **Client Secret** que recuperó anteriormente y pulse **Save**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. Haga clic en **Validar configuración de sincronización**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. Haga clic en **Siguiente**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. Debería ver todas las marcas de verificación verdes. Haga clic en **Cerrar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >Si ve una X roja entre sus marcas de verificación verdes, vea [este artículo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para ver las opciones de corrección.

1. Haga clic en **Habilitar sincronización**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

¡Y eso es todo!
