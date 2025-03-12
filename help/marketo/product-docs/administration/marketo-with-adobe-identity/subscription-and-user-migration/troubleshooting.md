---
description: Guía de solución de problemas de migración de usuarios de IMS de Adobe - Documentos de Marketo - Documentación del producto
title: Guía de solución de problemas de migración de usuarios de Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Guía de solución de problemas de migración de usuarios de Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Durante el proceso de migración de usuarios de IMS, se crea un usuario de Adobe para cada usuario de Marketo Engage que se migra (a menos que ya exista con la misma dirección de correo electrónico). A veces, no se crea, lo que puede atribuirse al registro del usuario en Active Directory o a problemas con la dirección de correo electrónico. Cuando esto sucede, el administrador de Marketo Engage ve el motivo en el campo de estado de migración del usuario en la consola de migración automática.

## Mensajes de error {#error-messages}

En primer lugar, determine si es necesario migrar al usuario o no, ya que esto afectará a los pasos de resolución que deben seguirse.

Utilice la sección &quot;En esta página&quot; a la derecha para ir directamente a un error específico.

### No está en el directorio {#not-in-directory}

**Causa raíz**: el usuario no existe en Active Directory (AD). Para cualquier organización con SSO que tenga habilitada la sincronización de AD, la creación de usuarios solo se permite mediante el proveedor de identidad (IdP). Como tal, no se pudo agregar el usuario a través de Admin Console durante la migración de usuarios.

**Resoluciones**:

_Si no es necesario migrar al usuario_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

_Si es necesario migrar al usuario_: un administrador del sistema debe agregar al usuario a Active Directory con los permisos adecuados. Administrador de Marketo Engage para volver a ejecutar la migración de este usuario desde la consola de migración.

### Carácter no válido de Gmail {#gmail-invalid-character}

**Causa raíz**: Según la directiva de seguridad de Adobe, los caracteres `.` y `+` no están permitidos en una dirección de correo electrónico de Gmail. Ambos caracteres están permitidos en direcciones de correo electrónico que no sean de Gmail.

**Resoluciones**:

_Si no es necesario migrar al usuario_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

_Si es necesario migrar al usuario_: la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir la directiva de seguridad de Adobe y debe volver a verificarse. Administrador de Marketo para volver a ejecutar la migración de este usuario desde la consola de migración.

### Usuario inactivo {#inactive-user}

**Causa raíz**: la sincronización de AD está habilitada y la cuenta federada del usuario existe pero en estado inactivo/deshabilitado.

**Resoluciones**:

_Si no es necesario migrar al usuario_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

_Si es necesario migrar al usuario_: se deben restaurar el estado y los permisos adecuados del usuario. Administrador de Marketo Engage para volver a ejecutar la migración de este usuario desde la consola de migración.

### No está en el dominio {#not-in-domain}

**Causa raíz**: la aplicación de dominios está habilitada en Admin Console, pero el dominio de la dirección de correo electrónico del usuario no es uno de los dominios permitidos.

**Resoluciones**:

_Si no es necesario migrar al usuario_, el administrador de Marketo Engage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

_Si es necesario migrar al usuario_: la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir con la directiva de aplicación de dominios (DE). Como alternativa, el administrador del sistema puede [mover el dominio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} a otro directorio deshabilitado de aplicación de dominio (DE) o [crear un nuevo directorio](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"} que no esté en la directiva DE. Administrador de Marketo Engage para volver a ejecutar la migración de este usuario desde la consola de migración.

### Error al crear {#create-failure}

**Causa raíz**: este error puede deberse a varios motivos en el servidor.

**Resoluciones**:

Envíe un caso de soporte con detalles relevantes para [Soporte de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

### Error de usuario Type2e {#type2e-user-failure}

**Causa raíz**: este error puede deberse a varios motivos en el servidor.

**Resoluciones**:

Envíe un caso de soporte con detalles relevantes para [Soporte de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
