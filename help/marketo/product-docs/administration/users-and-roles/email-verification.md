---
description: Verificación por correo electrónico - Documentos de Marketo - Documentación del producto
title: Verificación de correo electrónico
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 7b64e6e9bbd282b1e27f4c9c862df07642e9a35b
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Verificación de correo electrónico {#email-verification}

Las suscripciones a Adobe Marketo Engage requieren que todos los usuarios que no sean solo de API, incluidos los administradores de Marketo Engage, comprueben su dirección de correo electrónico.

## Por qué se introdujo esta función {#why-this-feature-was-introduced}

El Marketo Engage continúa con la implementación de la verificación por correo electrónico como preparación para migrar clientes a Adobe Business Platform, incluida la migración de usuarios a ID de Adobe. Esta función mejora la seguridad de las cuentas de usuario de Marketo Engage existentes. Para garantizar que un usuario Marketo Engage esté asociado con el Adobe ID adecuado, los usuarios Marketo Engage existentes deben comprobar su dirección de correo electrónico. Un usuario Marketo Engage debe tener una dirección de correo electrónico verificada para poder migrar a un Adobe ID. Si un usuario Marketo Engage no comprueba su dirección de correo electrónico, no puede migrarse a una Adobe ID y perderá el acceso a una suscripción de Marketo una vez completada la migración de usuario para la suscripción.

## Invitación de usuario {#user-invite}

Cuando un administrador invita a un usuario, este se verifica automáticamente una vez que hace clic en el vínculo de invitación.

>[!IMPORTANT]
>
>La excepción a lo anterior es, _en una suscripción de solo SSO_, los administradores recibirán una nueva invitación de usuario, pero los usuarios que no sean administradores no. Los usuarios que no son administradores deben seguir con el proceso de verificación por correo electrónico para garantizar la migración de sus registros. Los usuarios pueden enviarse el vínculo de verificación por correo electrónico si hacen clic en su icono de Perfil, acceden a **Mi cuenta** > **Configuración de la cuenta** y hacen clic en **Volver a enviar verificación**.

![](assets/email-verification-1.png)

## Verificación del correo electrónico {#verification-email}

Los usuarios recibirán el correo electrónico siguiente cuando se active la verificación por correo electrónico para una suscripción o si la activa un administrador/usuario.

Se requiere una sesión de usuario activa para que la verificación del correo electrónico se realice correctamente. En primer lugar, el usuario debe iniciar sesión en su suscripción de Marketo mediante la URL de su proveedor de identidad (IdP). Una vez establecida una sesión, _luego_ harían clic en el vínculo **Verificar dirección de correo electrónico** del correo electrónico.

![](assets/email-verification-2.png)

>[!TIP]
>
>Para reenviar un correo electrónico de verificación a un usuario no verificado, simplemente selecciona su registro y haz clic en el botón **[!UICONTROL Verificar correo electrónico]**.

## Cambio de una dirección de correo electrónico {#changing-an-email-address}

Cuando se cambia la dirección de correo electrónico de un usuario, pasa a estar sin verificar. Se les enviará un correo electrónico para que puedan volver a verificarlo. Los usuarios pueden reenviar manualmente ese correo electrónico haciendo clic en **[!UICONTROL Reenviar verificación]**.

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## Usuarios y funciones {#users-and-roles}

En **[!UICONTROL Administración]** > **[!UICONTROL Usuarios y roles]**, la columna Estado de correo electrónico muestra el estado de verificación de cada usuario.

![](assets/email-verification-5.png)

## ID de inicio de sesión de varios usuarios {#multiple-user-login-ids}

Solo se puede asociar una cuenta de usuario a una sola dirección de correo electrónico. Si hay varias cuentas de usuario asociadas a una sola dirección de correo electrónico, Marketo Engage requiere que se resuelva el conflicto y se muestren todos los inicios de sesión de usuario asociados a la dirección de correo electrónico, así como tres opciones de resolución:

* Usar el correo electrónico actual para el ID de inicio de sesión del usuario actual
* Usar un nuevo correo electrónico para el ID de inicio de sesión del usuario actual
* Retrasar la decisión hasta el siguiente inicio de sesión

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>Aunque una cuenta de usuario debe asociarse con una sola dirección, se puede utilizar una cuenta de usuario en muchas suscripciones mediante un ID universal.
