---
unique-page-id: 2360356
description: Añadir el inicio de sesión único en un portal - Documentos de marketing - Documentación del producto
title: Añadir el inicio de sesión único en un portal
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Añadir el inicio de sesión único en un portal {#add-single-sign-on-to-a-portal}

Si tiene un servicio de directorio que autentica usuarios, puede permitir el inicio de sesión único (SSO) en Marketing. Esta función es compatible con la versión 2.0 y posterior del Lenguaje de marcado de aserción de seguridad (SAML).

Marketing funciona como Proveedor de servicio SAML (SP) y depende de un proveedor de identidad externo (IdP) para autenticar a los usuarios.

Una vez activado el inicio de sesión único, el IdP puede validar las credenciales de un usuario. Cuando un usuario desea utilizar el software de Marketing, el IdP envía un mensaje SAML firmado a MarketingTo, que actúa como SP. Este mensaje garantiza a Marketing que el usuario está autorizado a utilizar el software de Marketing.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>¿Es usuario de Microsoft Azure? Consulte su [tutorial de integración](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Cómo enviar la solicitud {#how-to-send-the-request}

* Enviar la solicitud de SSO, que es una respuesta de SAML, a `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Como URL de Audiencia del SP. Use [https://saml.marketo.com/sp](https://saml.marketo.com/sp)
* Si utiliza el atributo SPNameQualifier, establezca el elemento NameID para Subject en [https://saml.marketo.com/sp](https://saml.marketo.com/sp)
* Si va a federar varias suscripciones de Marketing to al mismo proveedor de SSO, puede utilizar direcciones URL de SP únicas para cada proveedor de Marketing con el formato `https://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo solo admite los iniciados por el proveedor de identidad (también conocidos como iniciados por IdP), en los que el usuario inicia primero la página de inicio de sesión Idp, se autentica y luego navega a Mi marketing.

## Notas adicionales {#additional-notes}

* **Tiempo**  de sincronización: para un nuevo usuario, hay un retraso de unos 10 minutos antes de que se procese una solicitud de SSO inicial.
* **Aprovisionamiento**  de usuarios: los usuarios son aprovisionados manualmente por Marketing.
* **Autorización** : los permisos de usuario se mantienen dentro de Marketing.
* **Compatibilidad**  con OAuth: actualmente, Marketo no admite OAuth.

>[!NOTE]
>
>Antes de comenzar, tenga el certificado de proveedor de identidad en formato X.509 y en extensión .crt, .der o .cer.

## Actualizar la configuración de SAML {#update-saml-settings}

SSO está deshabilitado de forma predeterminada. Siga estos pasos para habilitar SAML y configurarlo.

1. Vaya a **Administración** y haga clic en **Inicio de sesión único**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Si no ve **Inicio de sesión único** en **Administración**, póngase en contacto con [[Soporte técnico de marketing]](https://nation.marketo.com/t5/Support/ct-p/Support).

1. En la sección **Configuración de SAML**, haga clic en **Editar**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Cambie **Inicio de sesión único de SAML** a **Habilitado**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Introduzca su **Id. de emisor**, **Id. de entidad**, seleccione la **Ubicación de ID de usuario** y haga clic en **Examinar**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Seleccione el archivo **Certificado de proveedor de identidad**.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Actualizar la configuración de la página de redirección {#update-redirect-page-settings}

1. En la sección **Redireccionar páginas**, haga clic en **Editar**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Los clientes que utilicen el identificador universal junto con el inicio de sesión único deben introducir la dirección URL de inicio de sesión del proveedor de identidad en el campo **URL de inicio de sesión**.

1. Introduzca una **URL de cierre de sesión**. Ésta es la dirección URL a la que desea que se dirija al usuario cuando cierre la sesión de Marketing.

   ![](assets/eight.png)

1. Escriba una **URL de error**. Es la dirección URL a la que desea que se dirija al usuario en caso de que falle el inicio de sesión en Marketing Cloud. Haga clic en **Guardar**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Ambas páginas deben estar disponibles para el público.
