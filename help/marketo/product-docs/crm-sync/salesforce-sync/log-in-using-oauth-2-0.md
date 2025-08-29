---
description: 'Inicio de sesión con OAuth 2.0: documentación de Marketo: documentación del producto'
title: Iniciar sesión con OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 3e007c6ddc150227310f2d38a7f77ad86ca15ffa
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Iniciar sesión con OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utiliza el protocolo OAuth para permitir a los usuarios de aplicaciones acceder a los datos de forma segura (autenticar la aplicación mediante OAuth 2.0) sin tener que revelar las credenciales de inicio de sesión. A continuación se indican los pasos que se deben seguir para conectar y sincronizar Marketo Engage de forma segura con Salesforce.

>[!IMPORTANT]
>
>Para conectar Marketo y [!DNL Salesforce] mediante OAuth, inicie sesión en Marketo a través del explorador privado (incógnito) para evitar conectarse a [!DNL Salesforce] con el nombre de usuario incorrecto.

## Configurar la aplicación conectada {#set-up-connected-app}

1. En Salesforce, en Configuración, en Herramientas de plataforma, navegue hasta Aplicaciones, Administrador de aplicaciones y haga clic en **[!UICONTROL Nueva aplicación conectada]**.

   ![](assets/setting-up-oauth-2-1.png)

1. Complete los detalles y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/setting-up-oauth-2-2.png)

1. Haga clic en la casilla de verificación **[!UICONTROL Habilitar la configuración de OAuth]**. Para URL de devolución de llamada, ingrese `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Seleccione todos los ámbitos de OAuth disponibles y haga clic en **[!UICONTROL Agregar]**.

   ![](assets/setting-up-oauth-2-3.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/setting-up-oauth-2-4.png)

1. Haga clic en **[!UICONTROL Continuar]**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copie la clave del consumidor y el secreto del consumidor (los necesitará más adelante para usarlos en Marketo Engage).

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>Mientras sigue en la página Nueva aplicación conectada, desplácese hacia abajo y asegúrese de que la casilla de verificación &quot;Requerir clave de prueba para intercambio de código (PKCE)&quot; esté _NO_ marcada, ya que interferiría con la configuración.

## Configuración de Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* El acceso a la API debe estar habilitado para el usuario de sincronización de Salesforce (si es usuario de Salesforce Professional Edition, ese acceso no está disponible de forma predeterminada; póngase en contacto con el administrador de cuentas de Salesforce).
>* El usuario de sincronización de Marketo debe crearse en Salesforce.
>* Para los clientes existentes, la función &quot;Habilitar OAuth para la sincronización de SFDC&quot; está habilitada en la suscripción del cliente.
>* Los bloqueadores de elementos emergentes están deshabilitados.
>* Se ha creado la aplicación conectada y tenemos [!UICONTROL Clave de consumidor] y [!UICONTROL Secreto de consumidor] disponibles para usar.

>[!CAUTION]
>
>Asegúrese de ocultar al usuario de sincronización todos los campos que no necesite en Marketo antes de hacer clic en **[!UICONTROL Campos de sincronización]**. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver en SFDC se crearán en Marketo de forma permanente y no se podrán eliminar.

1. En la sección Administración de Marketo, haz clic en **[!UICONTROL CRM]**, luego en **[!UICONTROL Sincronizar con Salesforce]**.

   ![](assets/setting-up-oauth-2-7.png)

1. Agregue la clave de consumidor y la información del secreto de consumidor que registró anteriormente, haga clic en y **[!UICONTROL Guardar]**.

   ![](assets/setting-up-oauth-2-8.png)

1. En la página de sincronización de Marketo Salesforce, haga clic en el botón **[!UICONTROL Iniciar sesión con Salesforce]**.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Si ve los campos Nombre de usuario/Contraseña/Token y no un botón &quot;Iniciar sesión con Salesforce&quot;, su suscripción a Marketo está habilitada para la autenticación básica. Consulte [Configurar Marketo con autenticación básica](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}. Una vez que la sincronización comienza con un conjunto de credenciales, no se cambia de credenciales de Salesforce ni de suscripción. Para que Oauth 2.0 esté configurado para la autenticación de Salesforce, comuníquese con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

1. Se mostrará una ventana emergente con la página de inicio de sesión de Salesforce. Introduzca sus credenciales de &quot;Usuario de sincronización de Marketo&quot; e inicie sesión.

   ![](assets/setting-up-oauth-2-10.png)

1. Escribe el código de verificación que recibiste por correo electrónico (enviado por Salesforce) y haz clic en **[!UICONTROL Verificar]**.

   ![](assets/setting-up-oauth-2-11.png)

1. Una vez verificada correctamente, aparecerá la página de acceso que solicita el acceso. Haga clic en **[!UICONTROL Permitir]**.

   ![](assets/setting-up-oauth-2-12.png)

1. En unos minutos, aparecerá una ventana emergente en Marketo. Haga clic en **[!UICONTROL Confirmar credenciales]**.

   ![](assets/setting-up-oauth-2-13.png)

1. Una vez finalizada la sincronización de campos, haga clic en **[!UICONTROL Iniciar sincronización de Salesforce]**.

   ![](assets/setting-up-oauth-2-14.png)

1. Haga clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/setting-up-oauth-2-15.png)

La sincronización entre Marketo y [!DNL Salesforce] está en curso.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Paso 1 de 3: agregar campos de Marketo a Salesforce (empresarial/ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Instalar el paquete Marketo Sales Insight en Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
