---
description: 'Inicio de sesión con OAuth 2.0: documentación de Marketo: documentación del producto'
title: Iniciar sesión con OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Iniciar sesión con OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utiliza el protocolo OAuth para permitir que los usuarios de aplicaciones accedan a los datos de forma segura (autentican la aplicación mediante OAuth 2.0) sin tener que revelar las credenciales de inicio de sesión. A continuación se indican los pasos que se deben seguir para conectarse y sincronizar Marketo de forma segura con Salesforce.

>[!IMPORTANT]
>
>Para conectar Marketo y Salesforce con OAuth, inicie sesión en Marketo a través del explorador privado (de incógnito) como para evitar conectarse a Salesforce con el nombre de usuario incorrecto.

## Configurar la aplicación conectada {#set-up-connected-app}

1. En Salesforce, en Configuración, dentro de las Herramientas de plataforma, navegue hasta Aplicaciones, Administrador de aplicaciones y haga clic en **Nueva aplicación conectada**.

   ![](assets/setting-up-oauth-2-1.png)

1. Complete los detalles y haga clic en **Guardar**.

   ![](assets/setting-up-oauth-2-2.png)

1. Haga clic en **Habilitar la configuración de OAuth** casilla de verificación En URL de devolución de llamada, introduzca `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Seleccione todos los ámbitos de OAuth disponibles y haga clic en **Añadir**.

   ![](assets/setting-up-oauth-2-3.png)

1. Clic **Guardar**.

   ![](assets/setting-up-oauth-2-4.png)

1. Clic **Continuar**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copie la Clave de consumidor y el Secreto del consumidor.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Guarde la clave del consumidor y la información del secreto del consumidor para usarlas más adelante en Marketo.

## Configuración de Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* El acceso a la API debe estar habilitado para el usuario de sincronización de Salesforce (si es usuario de Salesforce Professional Edition, ese acceso no está disponible de forma predeterminada; póngase en contacto con el ejecutivo de cuenta de Salesforce).
>* El usuario de sincronización de Marketo debe crearse en Salesforce.
>* Para los clientes existentes, la función &quot;Habilitar OAuth para la sincronización de SFDC&quot; está habilitada en la suscripción del cliente.
>* Los bloqueadores de elementos emergentes están deshabilitados.
>* La aplicación conectada se crea y tenemos la clave del consumidor y el secreto del consumidor disponibles para su uso.

>[!CAUTION]
>
>Asegúrese de ocultar al usuario de sincronización todos los campos que no necesite en Marketo antes de hacer clic en **Sincronizar campos**. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver en SFDC se crearán en Marketo de forma permanente y no se podrán eliminar.

1. En la sección Administración de Marketo, haga clic en **CRM**, entonces **Sincronizar con Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Añada la información de clave del consumidor y secreto del consumidor que ha registrado anteriormente y haga clic en y **Guardar**.

   ![](assets/setting-up-oauth-2-8.png)

1. En la página de sincronización de Marketo Salesforce, haga clic en **Iniciar sesión con Salesforce** botón.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Si ve los campos Nombre de usuario/Contraseña/Token y no un botón &quot;Iniciar sesión con Salesforce&quot;, su suscripción a Marketo estará habilitada para la autenticación básica. Consulte la [Configuración de Marketo con autenticación básica](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). Una vez que la sincronización comienza con un conjunto de credenciales, no se produce ningún cambio de credenciales o suscripción de Salesforce. Si desea utilizar Oauth 2.0, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas).

1. Se mostrará una ventana emergente con la página de inicio de sesión de Salesforce. Introduzca sus credenciales de &quot;Usuario de sincronización de Marketo&quot; e inicie sesión.

   ![](assets/setting-up-oauth-2-10.png)

1. Introduzca el código de verificación que recibió por correo electrónico (enviado por Salesforce) y haga clic en **Verificar**.

   ![](assets/setting-up-oauth-2-11.png)

1. Una vez verificada correctamente, aparecerá la página de acceso que solicita el acceso. Clic **Permitir**.

   ![](assets/setting-up-oauth-2-12.png)

1. En unos minutos, aparecerá una ventana emergente en Marketo. Clic **Confirmar credenciales**.

   ![](assets/setting-up-oauth-2-13.png)

1. Al finalizar la sincronización de campos, haga clic en **Iniciar sincronización de Salesforce**.

   ![](assets/setting-up-oauth-2-14.png)

1. Clic **Iniciar sincronización**.

   ![](assets/setting-up-oauth-2-15.png)

La sincronización entre Marketo y Salesforce ya está en curso.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Instalación del paquete de información de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
