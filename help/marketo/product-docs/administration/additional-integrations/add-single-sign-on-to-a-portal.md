---
unique-page-id: 2360356
description: Habilite el inicio de sesión único de SAML 2.0 para que su proveedor de identidad autentique a los usuarios en Marketo.
title: Añadir el inicio de sesión único a un portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
feature: Administration
TQID: https://experienceleague.adobe.com/-3bbSWs-yvF6QaXVzY5nJStkPqZtBttJu2EcDq5I3GE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 658
ht-degree: 5%

---

# Añadir el inicio de sesión único a un portal {#add-single-sign-on-to-a-portal}

Si tiene un servicio de directorio que autentica a los usuarios, puede permitir el inicio de sesión único (SSO) en Marketo. Marketo admite esta característica mediante [!DNL Security Assertion Markup Language] (SAML) versión 2.0 y posteriores.

Marketo funciona como un proveedor de servicios SAML (SP) y depende de un proveedor de identidad externo (IdP) para autenticar a los usuarios.

Una vez habilitado el SSO, el IdP puede validar las credenciales de un usuario. Cuando un usuario desea utilizar el software de Marketo, el IdP envía un mensaje SAML firmado a Marketo, que actúa como SP. Este mensaje confirma a Marketo que el usuario está autorizado a utilizar el software de Marketo.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!IMPORTANT]
>
>Esto no se aplica **not** a las suscripciones incorporadas a Adobe Identity. Es posible que aparezcan ajustes anteriores (anteriores a la migración de IMS), pero ya no se aplican. Para las suscripciones incorporadas a Adobe Identity, el inicio de sesión único [está configurado](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"} en el nivel de organización de Adobe en Adobe Admin Console.

>[!NOTE]
>
>¿Es un usuario de [!DNL Microsoft Azure]? Consulte su [tutorial de integración](https://learn.microsoft.com/en-us/entra/identity/saas-apps/marketo-tutorial){target="_blank"}. Tenga en cuenta que hay un error tipográfico en el paso 5c de su tutorial. Establecer el estado de retransmisión en `https://<munchkinid>.mktoweb.com`, **_no_** `https://<munchkinid>.marketo.com`.

## Cómo enviar la solicitud {#how-to-send-the-request}

* Enviar la solicitud SSO, que es una respuesta SAML, a `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Como URL de audiencia del SP. Usar `http://saml.marketo.com/sp`
* Si está usando el atributo SPNameQualifier, establezca el elemento NameID del asunto en `http://saml.marketo.com/sp`
* Si está federando varias suscripciones de Marketo al mismo proveedor de SSO, puede utilizar direcciones URL de SP únicas para cada subrutina de Marketo con el formato `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo solo admite el inicio del proveedor de identidad (también conocido como inicio de IdP), en el que el usuario inicia primero la página de inicio de sesión de IdP, se autentica y, a continuación, navega a Mi Marketo. Si la suscripción de Marketo se ha movido a Admin Console, Adobe Admin Console solo admite servicios iniciados por Service Provider (también conocidos como iniciados por SP) en este momento. Es posible que se hayan realizado cambios en su experiencia de SSO.

## Notas adicionales {#additional-notes}

* **Tiempo de sincronización**: para un usuario nuevo, hay un retraso de unos 10 minutos antes de que se procese una solicitud de SSO inicial.
* **Aprovisionamiento de usuarios**: Marketo aprovisiona a los usuarios manualmente.
* **Autorización**: los permisos de usuario se mantienen en Marketo.
* **Compatibilidad con OAuth**: Marketo no admite OAuth en este momento.
* **Propagación automática del usuario** - También conocida como &quot;Aprovisionamiento justo a tiempo&quot;, es cuando el primer inicio de sesión de SAML de un usuario puede crearlo en cualquier aplicación web a la que acceda (por ejemplo, Marketo) y no se requiere ninguna acción de administración manual. Esto no es compatible con Marketo en este momento.
* **Cifrado**: Marketo no admite actualmente el cifrado.

>[!NOTE]
>
>Antes de empezar, tenga el certificado de proveedor de identidad en formato X.509 y en la extensión .crt, .der o .cer.

## Actualizar configuración de SAML {#update-saml-settings}

SSO está desactivado de forma predeterminada. Siga estos pasos para habilitar SAML y configurarlo.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Haga clic en **[!UICONTROL Inicio de sesión único]**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Si no ve **[!UICONTROL Inicio de sesión único]** en **[!UICONTROL Administración]**, póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. En la sección **[!UICONTROL Configuración de SAML]**, haga clic en **[!UICONTROL Editar]**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Cambiar **[!UICONTROL inicio de sesión único de SAML]** a **[!UICONTROL Habilitado]**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Escriba su **[!UICONTROL ID de emisor]**, **[!UICONTROL ID de entidad]**, seleccione la **[!UICONTROL ubicación del ID de usuario]** y, a continuación, haga clic en **[!UICONTROL Examinar]**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Seleccione el archivo **[!UICONTROL Certificado de proveedor de identidad]**.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Actualizar configuración de página de redireccionamiento {#update-redirect-page-settings}

1. En la sección **[!UICONTROL Redirigir páginas]**, haga clic en **[!UICONTROL Editar]**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >Los clientes que usan el identificador universal junto con el SSO deben ingresar la URL de inicio de sesión del proveedor de identidad en el campo **[!UICONTROL URL de inicio de sesión]**.

1. Escriba una **[!UICONTROL URL de cierre de sesión]**. Dirección URL a la que desea que se dirija al usuario cuando cierre la sesión de Marketo.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Escriba una **[!UICONTROL URL con error]**. Dirección URL a la que desea que se dirija al usuario en caso de que falle el inicio de sesión en Marketo. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Ambas páginas deben estar disponibles para el público.

>[!MORELIKETHIS]
>
>* [Restringir el inicio de sesión del usuario solo a SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Invitar a usuarios de Marketo a dos instancias con identificador universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
