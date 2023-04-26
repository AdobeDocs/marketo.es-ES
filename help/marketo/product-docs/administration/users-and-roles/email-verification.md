---
description: Verificación de correo electrónico - Documentos de Marketo - Documentación del producto
title: Verificación de correo electrónico
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: c45b3ab94b806b53768891613f15b8e9b694a440
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Verificación de correo electrónico {#email-verification}

Las suscripciones a Adobe Marketo Engage requieren que todos los usuarios que no son solo de API, incluidos los administradores Marketo Engage, verifiquen su dirección de correo electrónico. Los usuarios con inicio de sesión único (SSO) a los que no se les asigne una función de administrador o a los que se les asigne una función con el permiso &quot;Omitir inicio de sesión único&quot; comprobarán automáticamente su correo electrónico cuando su suscripción esté habilitada con la función Verificación por correo electrónico.

**Invitación del usuario**

Cuando un administrador invita a un usuario, este se verifica automáticamente una vez que haga clic en el vínculo de invitación. Los usuarios de SSO, no asignados a la función de administrador, se verifican automáticamente.

**Cambio de una dirección de correo electrónico**

Cuando se cambia la dirección de correo electrónico de un usuario, no se verifica. Se les enviará un correo electrónico que les permitirá volver a verificar. Los usuarios pueden reenviar manualmente ese correo electrónico haciendo clic en **Verificación de reenvío**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

**Usuarios y funciones**

En Administración > Usuarios y funciones, la columna Estado del correo electrónico muestra el estado de verificación de cada usuario.

![](assets/email-verification-3.png)

Para reenviar un correo electrónico de verificación a un usuario sin verificar, simplemente seleccione su registro y haga clic en el botón **Comprobar correo electrónico** botón.
