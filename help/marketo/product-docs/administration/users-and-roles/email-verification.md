---
description: Verificación por correo electrónico - Documentos de Marketo - Documentación del producto
title: Verificación de correo electrónico
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: 44cca5ebad831cc39babac87ac9ebbf53df6c795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Verificación de correo electrónico {#email-verification}

Las suscripciones a Adobe Marketo Engage requieren que todos los usuarios que no sean solo de API, incluidos los administradores de Marketo Engage, comprueben su dirección de correo electrónico. A los usuarios de inicio de sesión único (SSO) que no se les asigne una función de administrador o que se les asigne una función con el permiso &quot;Omitir SSO&quot; se les verificará automáticamente su correo electrónico cuando su suscripción esté habilitada con la función de verificación por correo electrónico.

## Invitación de usuario {#user-invite}

Cuando un administrador invita a un usuario, este se verifica automáticamente una vez que hace clic en el vínculo de invitación. Los usuarios de SSO que no tengan asignada la función de administrador se verifican automáticamente.

## Cambio de una dirección de correo electrónico {#changing-an-email-address}

Cuando se cambia la dirección de correo electrónico de un usuario, pasa a estar sin verificar. Se les enviará un correo electrónico para que puedan volver a verificarlo. Los usuarios pueden reenviar manualmente ese correo electrónico haciendo clic en **Reenviar verificación**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

## Usuarios y funciones {#users-and-roles}

Entrada **Administrador** > **Usuarios y funciones**, la columna Estado de correo electrónico muestra el estado de verificación de cada usuario.

![](assets/email-verification-3.png)

## ID de inicio de sesión de varios usuarios {#multiple-user-login-ids}

Solo se puede asociar una cuenta de usuario a una sola dirección de correo electrónico. Si hay varias cuentas de usuario asociadas a una sola dirección de correo electrónico, Marketo Engage requiere que se resuelva el conflicto y se muestren todos los inicios de sesión de usuario asociados a la dirección de correo electrónico, así como tres opciones de resolución:<p>
`1` Usar el correo electrónico actual para el ID de inicio de sesión del usuario actual<p>
`2` Usar un nuevo correo electrónico para el ID de inicio de sesión del usuario actual<p>
`3` Retrasar la decisión hasta el siguiente inicio de sesión

![](assets/email-verification-4.png)

## Correo electrónico de verificación {#verification-email}

Los usuarios invitados recibirán el siguiente correo electrónico:

![](assets/email-verification-5.png)

>[!NOTE]
>
>Para reenviar un correo electrónico de verificación a un usuario no verificado, simplemente seleccione su registro y haga clic en **Verificar correo electrónico** botón.
