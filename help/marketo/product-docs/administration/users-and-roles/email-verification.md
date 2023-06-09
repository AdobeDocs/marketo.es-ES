---
description: Verificación por correo electrónico - Documentos de Marketo - Documentación del producto
title: Verificación de correo electrónico
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: 7c168abc79e88c9d90786c4d5b86acbc8e0423b6
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Verificación de correo electrónico {#email-verification}

Las suscripciones a Adobe Marketo Engage requieren que todos los usuarios que no sean solo de API, incluidos los administradores de Marketo Engage, comprueben su dirección de correo electrónico. A los usuarios de inicio de sesión único (SSO) que no se les asigne una función de administrador o que se les asigne una función con el permiso &quot;Omitir SSO&quot; se les verificará automáticamente su correo electrónico cuando su suscripción esté habilitada con la función de verificación por correo electrónico.

## Por qué se introdujo esta función {#why-this-feature-was-introduced}

El Marketo Engage continúa con la implementación de la verificación por correo electrónico como preparación para migrar clientes a Adobe Business Platform, incluida la migración de usuarios a ID de Adobe. Esta función mejora la seguridad de las cuentas de usuario de Marketo Engage existentes. Para garantizar que un usuario Marketo Engage esté asociado con el Adobe ID adecuado, los usuarios Marketo Engage existentes deben comprobar su dirección de correo electrónico. Un usuario Marketo Engage debe tener una dirección de correo electrónico verificada para poder migrar a un Adobe ID. Si un usuario Marketo Engage no comprueba su dirección de correo electrónico, no puede migrarse a una Adobe ID y perderá el acceso a una suscripción de Marketo una vez completada la migración de usuario para la suscripción.

## Invitación de usuario {#user-invite}

Cuando un administrador invita a un usuario, este se verifica automáticamente una vez que hace clic en el vínculo de invitación. Los usuarios de SSO que no tengan asignada la función de administrador se verifican automáticamente.

## Correo electrónico de verificación {#verification-email}

Los usuarios recibirán el siguiente correo electrónico cuando se active la verificación por correo electrónico para una suscripción o si la activa un administrador/usuario:

![](assets/email-verification-1.png)

>[!NOTE]
>
>Para reenviar un correo electrónico de verificación a un usuario no verificado, simplemente seleccione su registro y haga clic en **Verificar correo electrónico** botón.

## Cambio de una dirección de correo electrónico {#changing-an-email-address}

Cuando se cambia la dirección de correo electrónico de un usuario, pasa a estar sin verificar. Se les enviará un correo electrónico para que puedan volver a verificarlo. Los usuarios pueden reenviar manualmente ese correo electrónico haciendo clic en **Reenviar verificación**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## Usuarios y funciones {#users-and-roles}

Entrada **Administrador** > **Usuarios y funciones**, la columna Estado de correo electrónico muestra el estado de verificación de cada usuario.

![](assets/email-verification-4.png)

## ID de inicio de sesión de varios usuarios {#multiple-user-login-ids}

Solo se puede asociar una cuenta de usuario a una sola dirección de correo electrónico. Si hay varias cuentas de usuario asociadas a una sola dirección de correo electrónico, Marketo Engage requiere que se resuelva el conflicto y se muestren todos los inicios de sesión de usuario asociados a la dirección de correo electrónico, así como tres opciones de resolución:

* Usar el correo electrónico actual para el ID de inicio de sesión del usuario actual
* Usar un nuevo correo electrónico para el ID de inicio de sesión del usuario actual
* Retrasar la decisión hasta el siguiente inicio de sesión

  ![](assets/email-verification-5.png)

>[!NOTE]
>
>Aunque una cuenta de usuario debe asociarse con una sola dirección, se puede utilizar una cuenta de usuario en muchas suscripciones mediante un ID universal.
