---
unique-page-id: 2360356
description: Agregar el inicio de sesión único a un portal - Documentos de Marketo - Documentación del producto
title: Agregar el inicio de sesión único a un portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Agregar el inicio de sesión único a un portal {#add-single-sign-on-to-a-portal}

Si tiene un servicio de directorio que autentica a los usuarios, puede permitir el inicio de sesión único (SSO) en Marketo. Admitimos esta función mediante [!DNL Security Assertion Markup Language] (SAML) versión 2.0 y posteriores.

Marketo funciona como un proveedor de servicios SAML (SP) y depende de un proveedor de identidad externo (IdP) para autenticar a los usuarios.

Una vez habilitado el SSO, el IdP puede validar las credenciales de un usuario. Cuando un usuario desea utilizar el software de Marketo, el IdP envía un mensaje SAML firmado a Marketo, que actúa como SP. Este mensaje garantiza a Marketo que el usuario está autorizado a utilizar el software de Marketo.

>[!NOTE]
>
>**Permisos de administración necesarios**

>[!NOTE]
>
>¿Es usted? [!DNL Microsoft Azure] ¿usuario? Consulte sus [tutorial de integración](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/){target="_blank"}.

## Cómo enviar la solicitud {#how-to-send-the-request}

* Envíe la solicitud SSO, que es una respuesta SAML, a `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Como URL de audiencia del SP. Utilizar `http://saml.marketo.com/sp`
* Si está utilizando el atributo SPNameQualifier, establezca el elemento NameID para Subject en `http://saml.marketo.com/sp`
* Si está federando varias suscripciones de Marketo al mismo proveedor de SSO, puede utilizar direcciones URL de SP únicas para cada subgrupo de Marketo con el formato `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo solo admite el inicio del proveedor de identidad (también conocido como inicio de IdP), en el que el usuario inicia primero la página de inicio de sesión de Idp, se autentica y, a continuación, navega a Mi Marketo.

## Notas adicionales {#additional-notes}

* **Tiempo de sincronización** - Para un usuario nuevo, hay un retraso de unos 10 minutos antes de que se procese una solicitud de SSO inicial.
* **Aprovisionamiento de usuarios** : Marketo aprovisiona a los usuarios manualmente.
* **Autorización** : Los permisos de usuario se mantienen en Marketo.
* **Compatibilidad con OAuth** : Marketo no es compatible actualmente con OAuth.
* **Propagación automática de usuarios** - También conocido como &quot;Aprovisionamiento justo a tiempo&quot;, es cuando el primer inicio de sesión de SAML de un usuario es capaz de crearlo en cualquier aplicación web a la que acceda (por ejemplo, Marketo) y no se requiere ninguna acción de administración manual. Esto no es compatible con Marketo en este momento.
* **Cifrado** - Marketo no admite actualmente el cifrado.

>[!NOTE]
>
>Antes de empezar, tenga el certificado de proveedor de identidad en formato X.509 y en la extensión .crt, .der o .cer.

## Actualizar configuración de SAML {#update-saml-settings}

SSO está desactivado de forma predeterminada. Siga estos pasos para habilitar SAML y configurarlo.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Clic **[!UICONTROL Inicio de sesión único]**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Si no lo ve... **[!UICONTROL Inicio de sesión único]** bajo **[!UICONTROL Administrador]**, contacto [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. En el **[!UICONTROL Configuración de SAML]** , haga clic en **[!UICONTROL Editar]**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Cambiar **[!UICONTROL Inicio de sesión único de SAML]** hasta **[!UICONTROL Habilitado]**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Introduzca su **[!UICONTROL Identificador de emisor]**, **[!UICONTROL ID de entidad]**, seleccione la **[!UICONTROL Ubicación del ID de usuario]**, luego haga clic en **[!UICONTROL Examinar]**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Seleccione su **[!UICONTROL Certificado de proveedor de identidad]** archivo.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Clic **[!UICONTROL Guardar]**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Actualizar configuración de página de redireccionamiento {#update-redirect-page-settings}

1. En el **[!UICONTROL Redirigir páginas]** , haga clic en **[!UICONTROL Editar]**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >Los clientes que utilicen ID universal junto con SSO deben introducir la URL de inicio de sesión del proveedor de identidad en la **[!UICONTROL URL de inicio de sesión]** field.

1. Introduzca una **[!UICONTROL URL de desconexión]**. Dirección URL a la que desea que se dirija al usuario cuando cierre la sesión de Marketo.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Introduzca una **[!UICONTROL URL de error]**. Dirección URL a la que desea que se dirija al usuario en caso de que falle el inicio de sesión en Marketo. Clic **[!UICONTROL Guardar]**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Ambas páginas deben estar disponibles para el público.

>[!MORELIKETHIS]
>
>* [Uso de un ID universal para el inicio de sesión con suscripción](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [Restringir el inicio de sesión del usuario a solo SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Invitación de usuarios de Marketo a dos instancias con ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
