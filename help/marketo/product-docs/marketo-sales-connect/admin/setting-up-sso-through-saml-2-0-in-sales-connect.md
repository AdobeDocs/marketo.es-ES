---
unique-page-id: 14352405
description: Configuración de SSO mediante SAML 2.0 en Sales Connect - Documentos de marketing - Documentación del producto
title: Configuración de SSO mediante SAML 2.0 en Sales Connect
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Configuración de SSO mediante SAML 2.0 en Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Se admite SSO mediante la especificación SAML 2.0. Sin embargo, no tenemos integraciones directas con ningún proveedor en este momento. Necesitaremos recopilar información de su proveedor de SSO para obtener esta configuración.

>[!NOTE]
>
>Esto solo se aplica a los clientes de **Marketing Sales Connect**. Si no dispone de Sales Connect pero desea obtener más información, póngase en contacto con el administrador de éxito del cliente.

## Requisitos {#requirements}

* Cuenta de SSO
* Suscripción de conexión de marketing a ventas
* Metadata.xml de la cuenta SSO (URL de problema, punto final para validación y clave pública)

## Configuración {#setup}

El archivo metadata.xml de la instancia de SSO de su equipo debe contener la dirección URL del emisor, el punto final para la validación y una clave pública.

También necesitaremos la ubicación SSO para que la cuenta SSO de su compañía sea un dominio único. Por ejemplo, se requiere un subdominio único como `toutapp.pingidentity.com` o similar. Sin este tipo de identificador único, no podremos configurar SAML desde el panel.

Un inicio de sesión y Okta no siempre proporcionan identificadores únicos al asignar una dirección URL. Si utiliza Okta o un inicio de sesión significa que no podremos configurar un inicio de sesión desde el botón de panel. Todavía podremos configurarlo desde el botón Registro único en la [aplicación Web](https://toutapp.com/login).

Una vez que tengamos esa información, trabajaremos con nuestro equipo de ingeniería para configurar esto para su suscripción.
