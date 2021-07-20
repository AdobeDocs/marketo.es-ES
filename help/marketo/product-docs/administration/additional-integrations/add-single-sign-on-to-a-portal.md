---
unique-page-id: 2360356
description: 'Adición del inicio de sesión único a un portal: Marketo Docs: documentación del producto'
title: Agregar el inicio de sesión único a un portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Agregar el inicio de sesión único a un portal {#add-single-sign-on-to-a-portal}

Si tiene un servicio de directorio que autentica a los usuarios, puede permitir el inicio de sesión único (SSO) en Marketo. Esta función es compatible con el uso de la versión 2.0 (o superior) del lenguaje de marcado de aserción de seguridad (SAML).

Marketo funciona como proveedor de servicios (SP) de SAML y depende de un proveedor de identidad (IdP) externo para autenticar a los usuarios.

Una vez habilitado el SSO, el IdP puede validar las credenciales de un usuario. Cuando un usuario desea utilizar software de Marketo, el IdP envía un mensaje SAML firmado a Marketo, actuando como SP. Este mensaje garantiza a Marketo que el usuario está autorizado a utilizar el software de Marketo.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>¿Es usuario de Microsoft Azure? Consulte su [tutorial de integración](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Cómo enviar la solicitud {#how-to-send-the-request}

* Envíe la solicitud de SSO, que es una respuesta de SAML, a `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Como URL de audiencia del SP. Usar `http://saml.marketo.com/sp`
* Si utiliza el atributo SPNameQualifier , establezca el elemento NameID para Subject en `http://saml.marketo.com/sp`
* Si está federando varias suscripciones de Marketo al mismo proveedor de SSO, puede utilizar direcciones url de SP únicas para cada subgrupo de Marketo con el formato `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo solo admite los mensajes iniciados por el proveedor de identidad (también conocidos como iniciados por IdP), en los que el usuario inicia primero la página de inicio de sesión de Idp, se autentica y, a continuación, navega a Mi Marketo.

## Notas adicionales {#additional-notes}

* **Tiempo de sincronización** : para un nuevo usuario, hay unos 10 minutos de retraso antes de que se procese una solicitud de SSO inicial.
* **Aprovisionamiento de usuarios** : Marketo aprovisiona los usuarios manualmente.
* **Autorización** : los permisos de usuario se mantienen en Marketo.
* **Compatibilidad con OAuth** : Marketo no es compatible actualmente con OAuth.
* **Propagación automática de usuarios** : también conocida como &quot;Aprovisionamiento justo a tiempo&quot;, es cuando el primer inicio de sesión de SAML de un usuario es capaz de crear al usuario en cualquier aplicación web a la que acceda (por ejemplo, Marketo) y no se requiere ninguna acción de administración manual. Marketo no lo admite en este momento.
* **Cifrado** : Marketo no admite actualmente el cifrado.

>[!NOTE]
>
>Antes de comenzar, pida al certificado de proveedor de identidad en formato X.509 y en extensión .crt, .der o .cer.

## Actualizar la configuración de SAML {#update-saml-settings}

SSO está desactivado de forma predeterminada. Siga estos pasos para habilitar SAML y configurarlo.

1. Vaya a **Admin** y haga clic en **Inicio de sesión único**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Si no ve **Inicio de sesión único** en **Administración**, póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. En la sección **Configuración de SAML**, haga clic en **Editar**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Cambie **Inicio de sesión único SAML** por **Habilitado**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Introduzca su **ID de emisor**, **ID de entidad**, seleccione la **Ubicación de ID de usuario** y haga clic en **Examinar**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Seleccione su archivo **Identity Provider Certificate**.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Actualizar la configuración de la página de redirección {#update-redirect-page-settings}

1. En la sección **Páginas de redireccionamiento**, haga clic en **Editar**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Los clientes que utilizan ID universal junto con SSO deben introducir la URL de inicio de sesión del proveedor de identidad en el campo **Login URL**.

1. Introduzca una **URL de cierre de sesión**. Esta es la dirección URL a la que desea que se dirija al usuario cuando cierre la sesión de Marketo.

   ![](assets/eight.png)

1. Introduzca una **URL de error**. Esta es la dirección URL a la que desea que se dirija al usuario en caso de que falle el inicio de sesión en Marketo. Haga clic en **Guardar**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Ambas páginas deben estar disponibles para el público.

>[!MORELIKETHIS]
>
>* [Uso de un ID universal para el inicio de sesión de suscripción](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
* [Restringir el inicio de sesión del usuario solo a SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
* [Invitación de usuarios de Marketo a dos instancias con ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

