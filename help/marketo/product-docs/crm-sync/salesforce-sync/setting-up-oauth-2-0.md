---
description: Configuración de OAuth 2.0 - Marketo Docs - Documentación del producto
title: Configuración de OAuth 2.0
translation-type: tm+mt
source-git-commit: 2d03d93e120c8b3ce359c6aca44730cfa7c16bf9
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Configuración de OAuth 2.0 {#setting-up-oauth-2-0}

Salesforce utiliza el protocolo OAuth para permitir que los usuarios de aplicaciones accedan de forma segura a los datos (autentique la aplicación mediante OAuth 2.0) a través de llamadas a la API REST sin tener que revelar las credenciales de inicio de sesión. A continuación se muestran los pasos que se deben realizar para conectar y sincronizar de forma segura Marketo con Salesforce.

## Configurar aplicación conectada {#set-up-connected-app}

1. En Salesforce, en Configuración, dentro de las Herramientas de plataforma, vaya a Aplicaciones, Administrador de aplicaciones y haga clic en **Nueva aplicación conectada**.

   ![](assets/setting-up-oauth-2-1.png)

1. Complete los detalles y haga clic en **Guardar**.

   ![](assets/setting-up-oauth-2-2.png)

1. Haga clic en la casilla **Habilitar configuración de OAuth**. Para Callback URL, escriba `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Seleccione todos los ámbitos de OAuth disponibles y haga clic en **Agregar**.

   ![](assets/setting-up-oauth-2-3.png)

1. Haga clic en **Guardar**.

   ![](assets/setting-up-oauth-2-4.png)

1. Haga clic en **Continue**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copie la clave de consumidor y el secreto del consumidor.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Guarde la clave del consumidor y la información del secreto del consumidor para usarla más adelante en Marketo.

## Configurar Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* El acceso a la API debe estar habilitado para el usuario de sincronización de Salesforce (si es usuario de Salesforce Professional Edition, ese acceso no está disponible de forma predeterminada; póngase en contacto con su ejecutivo de cuentas de Salesforce).
>* El usuario de Marketo Sync debe crearse en Salesforce.
>* Para los clientes existentes, la función &quot;Habilitar OAuth para la sincronización SFDC&quot; está habilitada en la suscripción del cliente.
>* Los bloqueadores de ventanas emergentes están desactivados.
>* La aplicación conectada se crea y tenemos la clave del consumidor y el secreto del consumidor disponibles para su uso.


1. En la sección Administración de Marketo, haga clic en **CRM** y luego en **Sincronizar con Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Agregue la información de la clave de consumidor y del secreto de consumidor que haya registrado anteriormente y haga clic en y **Guardar**.

   ![](assets/setting-up-oauth-2-8.png)

1. En la página de sincronización de Marketo Salesforce, haga clic en el botón **Login with Salesforce**.

   ![](assets/setting-up-oauth-2-9.png)

1. Aparecerá una ventana emergente con la página de inicio de sesión de salesforce. Clave en sus credenciales de &quot;usuario de sincronización de Marketo&quot; e inicie sesión.

   ![](assets/setting-up-oauth-2-10.png)

1. Introduzca el código de verificación que ha recibido por correo electrónico (enviado por Salesforce) y haga clic en **Verify**.

   ![](assets/setting-up-oauth-2-11.png)

1. Cuando la verificación se realice correctamente, la página de acceso mostrará la solicitud de acceso. Haga clic en **Permitir**.

   ![](assets/setting-up-oauth-2-12.png)

1. En unos minutos, aparecerá una ventana emergente en Marketo. Haga clic en **Confirmar credenciales**.

   ![](assets/setting-up-oauth-2-13.png)

1. Una vez finalizada la sincronización de campos, haga clic en **Iniciar sincronización de Salesforce**.

   ![](assets/setting-up-oauth-2-14.png)

1. Haga clic en **Iniciar sincronización**.

   ![](assets/setting-up-oauth-2-15.png)

La sincronización entre Marketo y Salesforce está en curso.

![](assets/setting-up-oauth-2-16.png)
