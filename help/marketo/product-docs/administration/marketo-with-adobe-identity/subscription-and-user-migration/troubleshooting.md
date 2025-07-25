---
description: Guía de solución de problemas de migración de usuarios de IMS de Adobe - Documentos de Marketo - Documentación del producto
title: Guía de solución de problemas de migración de usuarios de Adobe IMS
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e95748ed9a26f5454c342c6f6a9c29ec687c7cad
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 1%

---

# Guía de solución de problemas de migración de usuarios de Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Durante el proceso de migración de usuarios de IMS, se crea un usuario de Adobe para cada usuario de Marketo Engage que se migra (a menos que ya exista con la misma dirección de correo electrónico). A veces, no se crea, lo que puede atribuirse al registro del usuario en Active Directory o a problemas con la dirección de correo electrónico.

Este artículo, para los usuarios que realizan migraciones automáticas, enumera cada mensaje de error que puede ver en el campo de estado de la consola de migración automática.

>[!NOTE]
>
>Los errores relacionados con el directorio/dominio pueden activarse mediante otra organización/Admin Console en la que se haya configurado una confianza de directorio o en la que se haya reclamado el dominio.

## Mensajes de error {#error-messages}

En primer lugar, determine si es necesario migrar al usuario o no, ya que esto afectará a los pasos de resolución que deben seguirse.

Utilice la sección &quot;En esta página&quot; a la derecha para ir directamente a un error específico.

### Carácter no válido de Gmail {#gmail-invalid-character}

**Causa raíz**: Según la directiva de seguridad de Adobe, los caracteres `.` y `+` no están permitidos en una dirección de correo electrónico de Gmail. Ambos caracteres están permitidos en direcciones de correo electrónico que no sean de Gmail.

**Resoluciones**:

_Si es necesario migrar al usuario_: la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir la directiva de seguridad de Adobe y debe volver a verificarse. Administrador de Marketo para volver a ejecutar la migración de este usuario desde la consola de migración.

_Si el usuario hace **not**&#x200B;debe migrarse_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

### Usuario no incluido en el directorio {#user-not-in-directory}

**Causa raíz**: el usuario no existe en Active Directory (AD). Para cualquier organización con SSO que tenga habilitada la sincronización de AD, la creación de usuarios solo se permite mediante el proveedor de identidad (IdP). Como tal, no se pudo agregar el usuario a través de Admin Console durante la migración de usuarios.

**Resoluciones**:

_Si es necesario migrar al usuario_: un administrador del sistema debe agregar al usuario a Active Directory con los permisos adecuados. Administrador de Marketo Engage para volver a ejecutar la migración de este usuario desde la consola de migración.

_Si el usuario hace **not**&#x200B;debe migrarse_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

### Usuario inactivo {#inactive-user}

**Causa raíz**: la sincronización de AD está habilitada y la cuenta federada del usuario existe pero en estado inactivo/deshabilitado.

**Resoluciones**:

_Si es necesario migrar al usuario_: un administrador del sistema debe restaurar el estado y los permisos adecuados del usuario. Administrador de Marketo Engage para volver a ejecutar la migración de este usuario desde la consola de migración.

_Si el usuario hace **not**&#x200B;debe migrarse_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

### Dominio no válido {#invalid-domain}

**Causa raíz**: la aplicación del dominio está habilitada en Admin Console. Sin embargo, el dominio de la dirección de correo electrónico del usuario no es uno de los dominios permitidos o el dominio se ha reclamado en otra organización o Admin Console.

**Resoluciones**:

_Si es necesario migrar al usuario_ (y la aplicación del dominio está habilitada en la organización de migración), la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir con la directiva de aplicación de dominio (DE). Como alternativa, el administrador del sistema puede [mover el dominio](https://helpx.adobe.com/es/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} a otro directorio deshabilitado de aplicación de dominio (DE) o [crear un nuevo directorio](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"} que no esté en la directiva DE. Administrador de Marketo Engage para volver a ejecutar la migración de este usuario desde la consola de migración.

_Si es necesario migrar al usuario_ (y la aplicación del dominio está habilitada en otra organización), un administrador del sistema de la organización en la que se ha reclamado el dominio debe agregar la dirección de correo electrónico del usuario a la lista de excepciones. Administrador de Marketo Engage para volver a ejecutar la migración de este usuario desde la consola de migración.

_Si el usuario hace **not**&#x200B;debe migrarse_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

### Error de Type2E {#type2e-failure}

**Causa raíz**: error al crear una cuenta de usuario federada (para el inicio de sesión único) durante la migración de usuarios porque ya existe un Adobe ID para la misma dirección de correo electrónico que un usuario individual.

**Resoluciones**:

1. Elimine el usuario individual de la organización de Adobe. Tenga en cuenta que el usuario perderá el acceso a todos los productos y deberá volver a tener derecho a ellos más tarde.
1. Vuelva a ejecutar la migración de usuarios para crear una cuenta de usuario federada para este usuario.
1. Vuelva a añadir el usuario a los productos a los que tenía acceso anteriormente.

### Error al crear usuario {#user-creation-failed}

[Consulte a continuación](#failed)

### Hubo un error en el permiso de Marketo {#marketo-entitlement-failed}

[Consulte a continuación](#failed)

### Se produjo un error en el valor de la migración {#pendo-migration-failed}

[Consulte a continuación](#failed)

### Error de migración de datos de usuario {#user-data-migration-failed}

[Consulte a continuación](#failed)

### Error de sincronización de datos del producto {#product-data-sync-failed}

[Consulte a continuación](#failed)

### Error de derecho de Adobe {#adobe-entitlement-failed}

[Consulte a continuación](#failed)

### Error de cierre de sesión del usuario {#user-sign-out-failed}

[Consulte a continuación](#failed)

### Error de creación de Adobe ID {#adobe-id-creation-failed}

[Consulte a continuación](#failed)

### Error {#failed}

**Causa raíz**: estos errores pueden deberse a varios motivos en el servidor.

**Resoluciones**:

Envíe un caso de soporte con detalles relevantes para [Soporte de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
