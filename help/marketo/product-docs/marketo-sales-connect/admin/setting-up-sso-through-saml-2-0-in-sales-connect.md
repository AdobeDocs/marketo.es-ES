---
unique-page-id: 14352405
description: Configuración de SSO a través de SAML 2.0 en Sales Connect - Documentos de Marketo - Documentación del producto
title: Configuración de SSO a través de SAML 2.0 en Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Configuración de SSO a través de SAML 2.0 en Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Admitimos SSO mediante la especificación SAML 2.0. Sin embargo, no tenemos integraciones directas con ningún proveedor en este momento. Tendremos que recopilar cierta información de su proveedor de SSO para conseguir esta configuración.

>[!NOTE]
>
>Esto solo es aplicable a **usuarios de Marketo Sales Connect**. Si no dispone de Sales Connect pero desea obtener más información, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas).

## Requisitos {#requirements}

* cuenta SSO
* Suscripción a Marketo Sales connect
* Metadata.xml desde la cuenta SSO (dirección URL del problema, el punto final para la validación y una clave pública)

## Instalación {#setup}

El archivo metadata.xml de la instancia SSO de su equipo debe contener la dirección URL del emisor, el punto final para la validación y una clave pública.

También necesitaremos la Ubicación de SSO para que la cuenta de SSO de su compañía sea un dominio único. Por ejemplo, se requiere un subdominio único como `toutapp.pingidentity.com` o similar. Sin este tipo de identificador único, no podremos configurar SAML desde el panel.

One Login y Okta no siempre proporcionan identificadores únicos al asignar una dirección URL. Si utiliza Okta o un inicio de sesión, significa que no podremos configurar un inicio de sesión desde el botón del panel. Aún podremos configurarlo desde el botón Inicio de sesión único de la [aplicación web](https://toutapp.com/login).

Una vez que tengamos esa información, trabajaremos con nuestro equipo de ingeniería para configurarla para su suscripción.
