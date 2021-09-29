---
description: Configuración inicial - Documentos de Marketo - Documentación del producto
title: Configuración inicial
hide: true
hidefromtoc: true
source-git-commit: fe4a4b89ee295d8e351587a5ac858806a83f1305
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Configuración inicial {#initial-setup}

## Admin Console de acceso {#access-admin-console}

Siga los pasos a continuación para configurar el chat dinámico.

>[!NOTE]
>
>**Se requieren permisos de administrador.**

1. Una vez habilitado el chat dinámico para la instancia de Marketo, el administrador del sistema designado recibirá un correo electrónico de bienvenida. En ese correo electrónico, haga clic en **Introducción**.

   ![](assets/initial-setup-1.png)

1. Si anteriormente ha accedido a una aplicación con un Adobe ID, se le redirigirá directamente a Adobe Admin Console. Si no es así, [configure su Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html).

   ![](assets/initial-setup-2.png)

## Agregar usuarios {#add-users}

1. Después de iniciar sesión en el Admin Console, lo siguiente que hay que hacer es agregar usuarios. Tenemos ese proceso [documentado aquí](/help/marketo/product-docs/demand-generation/dynamic-chat/add-or-remove-chat-users.md#add-a-chat-user).

## Añadir permisos en Marketo {#add-permissions-in-marketo}

Después de agregar usuarios en el Admin Console , debe otorgar permisos en Marketo para que tengan acceso al acceso directo de chat dinámico desde Marketo.

1. En Marketo, haga clic en **Admin**.

1. Busque y haga doble clic en el usuario que desee.

1. Agregue **Acceso a Dynamic Chat** y haga clic en **Guardar**.

>[!IMPORTANT]
>
>Asegúrese de seguir los pasos en el orden indicado arriba. Si a alguien se le concede primero permiso en Marketo, verá el mosaico de Dynamic Chat pero no tendrá acceso de usuario.

El siguiente paso es [conectar Dynamic Chat a Marketo](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md).
