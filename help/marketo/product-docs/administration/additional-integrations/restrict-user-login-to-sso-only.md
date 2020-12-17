---
unique-page-id: 2360358
description: Restringir el inicio de sesión de usuario a SSO solamente - Documentos de marketing - Documentación del producto
title: Restringir el inicio de sesión de usuario sólo a SSO
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Restringir el inicio de sesión de usuario a SSO solamente {#restrict-user-login-to-sso-only}

Si está [usando SSO](add-single-sign-on-to-a-portal.md) y desea asegurarse de que los usuarios no pueden evitar la seguridad SSO, siga estas instrucciones.

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya a Administración y haga clic en Configuración de inicio de sesión.

![](assets/image2014-9-24-14-3a44-3a40.png)

1. Haga clic en Editar configuración de seguridad.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Expanda la configuración avanzada, marque Requerir SSO y haga clic en Guardar.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>Si selecciona **Requerir SSO**, puede excluir una [función de usuario](../../../product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de esta restricción marcando la opción **Omitir el inicio de sesión único** al configurar la función. Esto permitirá a los usuarios iniciar sesión con normalidad. Por ejemplo, es posible que los usuarios administradores necesiten iniciar sesión en Marketing a través de la pantalla de inicio de sesión.

>[!CAUTION]
>
>Cuando se invita a nuevos usuarios, reciben correos electrónicos de invitación. Sin embargo, si **Requerir SSO** está seleccionado, no recibirán estos mensajes de correo electrónico, a menos que estén asignados a una función que esté configurada como **Omitir el inicio de sesión único**.

¡Eso es todo! Ahora todos los usuarios (excepto los usuarios con permiso para omitir el inicio de sesión único) estarán restringidos a usar solo el inicio de sesión SSO.