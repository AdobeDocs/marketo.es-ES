---
unique-page-id: 2360358
description: 'Restringir el inicio de sesión del usuario solo a SSO: documentos de Marketo, documentación del producto'
title: Restringir el inicio de sesión del usuario a solo SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 5%

---

# Restringir el inicio de sesión del usuario a solo SSO {#restrict-user-login-to-sso-only}

Si está [usando SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) y desea asegurarse de que los usuarios no puedan saltarse la seguridad de SSO, siga estas instrucciones.

>[!IMPORTANT]
>
>Este artículo no se aplica a [Suscripciones de Marketo habilitadas para Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md).

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Haga clic en **[!UICONTROL Configuración de inicio de sesión]**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Haga clic en **[!UICONTROL Editar configuración de seguridad]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Expanda la configuración de **[!UICONTROL Advanced]**, marque **[!UICONTROL Requerir SSO]** y haga clic en **[!UICONTROL Guardar]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Una práctica recomendada es que se invite a los usuarios y que acepten la invitación. _Después_ de aceptar la invitación, los administradores deben establecerla en &quot;[!UICONTROL Requerir SSO]&quot;.

>[!TIP]
>
>Si selecciona **[!UICONTROL Requerir SSO]**, puede excluir un [rol de usuario](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de esta restricción marcando la opción **[!UICONTROL Omitir el inicio de sesión único]** al configurar el rol. Esto permitirá a los usuarios iniciar sesión normalmente. Por ejemplo, es posible que los usuarios administradores tengan que iniciar sesión en Marketo a través de la pantalla de inicio de sesión. Si tanto SSO como Universal ID están activados, debe tener el permiso &quot;Omitir el inicio de sesión único&quot; establecido para alternar entre suscripciones.

>[!CAUTION]
>
>Cuando se invita a nuevos usuarios, reciben correos electrónicos de invitación. Sin embargo, si se selecciona **[!UICONTROL Requerir SSO]**, no recibirán estos mensajes de correo electrónico, a menos que estén asignados a una función que esté establecida en **[!UICONTROL Omitir el inicio de sesión único]**.

¡Ya está! Ahora todos los usuarios (excepto los usuarios con permiso para omitir el inicio de sesión único) estarán restringidos a utilizar solo el inicio de sesión SSO.

>[!MORELIKETHIS]
>
>* [Agregar inicio de sesión único a un portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Usando un identificador universal para el inicio de sesión con suscripción](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitar a usuarios de Marketo a dos instancias con identificador universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
