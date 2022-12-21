---
unique-page-id: 14352405
description: Configuración de SSO mediante SAML 2.0 en Sales Connect - Marketo Docs - Documentación del producto
title: Configuración de SSO mediante SAML 2.0 en Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Configuración de SSO mediante SAML 2.0 en Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Se admite SSO a través de la especificación SAML 2.0. Sin embargo, no tenemos integraciones directas con ningún proveedor en este momento. Para obtener esta configuración, tendremos que recopilar información de su proveedor de SSO.

>[!NOTE]
>
>Esto solo es aplicable a **Marketo Sales Connect** clientes. Si no dispone de Conexión de ventas pero desea obtener más información, póngase en contacto con el gestor de éxito de los clientes.

## Requisitos {#requirements}

* Cuenta SSO
* suscripción de conexión de Marketo Sales
* Metadata.xml de la cuenta SSO (URL del problema, el punto final para la validación y una clave pública)

## Instalación {#setup}

El metadata.xml de la instancia SSO de su equipo debe contener la dirección URL del emisor, el punto final para la validación y una clave pública.

También necesitamos la ubicación SSO para que la cuenta SSO de su empresa sea un dominio único. Por ejemplo, se requiere un subdominio único como `toutapp.pingidentity.com` o similar. Sin este tipo de identificador único, no podremos configurar SAML desde el panel.

Un inicio de sesión y Okta no siempre proporcionan identificadores únicos al asignar una dirección URL. Si utiliza Okta o un inicio de sesión, significa que no podremos configurar un inicio de sesión desde el botón del panel. Todavía podremos configurarlo desde el botón Inicio de sesión único de la [aplicación web](https://toutapp.com/login).

Una vez que tengamos esa información, trabajaremos con nuestro equipo de ingeniería para configurarla para su suscripción.
