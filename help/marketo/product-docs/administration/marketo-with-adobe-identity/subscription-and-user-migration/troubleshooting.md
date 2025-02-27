---
description: Guía de solución de problemas de IMS de Adobe - Documentos de Marketo - Documentación del producto
title: Guía de resolución de problemas de Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: a2186f054e7b7a780098157927651a084e353bd8
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Guía de resolución de problemas de Adobe IMS {#adobe-ims-troubleshooting-guide}

Durante el proceso de migración de usuarios de IMS, se crea un usuario de Adobe para cada usuario de Marketo Engage que se migra. A veces, no se crea (por varios motivos, relacionados con el registro del usuario en Active Directory o problemas con la dirección de correo electrónico). Cuando esto sucede, el administrador de Marketo Engage ve el motivo en el campo de estado de migración del usuario en la consola de migración automática.

## Mensajes de error {#error-messages}

Utilice la sección &quot;En esta página&quot; a la derecha para ir directamente a un error específico y aprender a resolverlo.

### No está en el directorio {#not-in-directory}

_Causa raíz_: el usuario no existe en Active Directory (AD). Para cualquier organización con SSO que tenga habilitada la sincronización de AD, la creación de usuarios solo se permite mediante el proveedor de identidad (IdP). Como tal, no se pudo agregar el usuario a través de Admin Console durante la migración de usuarios.

_Resoluciones_:

Premigración: el administrador de Marketo Enage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

Después de la migración: el usuario debe agregarse a Active Directory con los permisos adecuados. El administrador de Marketo Engage debe volver a ejecutar la migración de este usuario desde la consola de migración.

### Carácter no válido de Gmail {#gmail-invalid-character}

_Causa raíz_: Por la directiva de seguridad de Adobe, los caracteres `.` y `+` no están permitidos en una dirección de correo electrónico de Gmail. Ambos caracteres solo se permiten en direcciones de correo electrónico que no sean de Gmail.

_Resoluciones_:

Premigración: el administrador de Marketo Enage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

Después de la migración: la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir con la política de seguridad de Adobe. Administrador de Marketo para volver a ejecutar la migración de este usuario desde la consola de migración.

### Usuario inactivo {#inactive-user}

_Causa raíz_: la sincronización de AD está habilitada y la cuenta federada del usuario existe pero en estado inactivo/deshabilitado.

_Resoluciones_:

Premigración: el administrador de Marketo Enage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

Después de la migración: se deben restaurar el estado y los permisos adecuados del usuario. El administrador de Marketo Engage debe volver a ejecutar la migración de este usuario desde la consola de migración.

### No está en el dominio {#not-in-domain}

_Causa raíz_: la aplicación de dominios está habilitada en Admin Console, pero el dominio de la dirección de correo electrónico del usuario no es uno de los dominios permitidos.

_Resoluciones_:

Premigración: el administrador de Marketo Enage omitirá al usuario en la consola de migración. El botón &quot;Migración completada&quot; aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en el botón para concluir el proceso de migración de usuarios.

Después de la migración: la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir con la política de aplicación de dominios (DE). Como alternativa, el administrador del sistema puede [mover el dominio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} a otro directorio deshabilitado de aplicación de dominio (DE) o [crear un nuevo directorio](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"} que no esté en la directiva DE. El administrador de Marketo Engage debe volver a ejecutar la migración de este usuario desde la consola de migración.

### Error al crear {#create-failure}

_Causa raíz_: este error puede deberse a varios motivos en el servidor.

_Resoluciones_:

Antes de la migración: envíe un caso de asistencia para los [que aún no se han migrado](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Después de la migración: envíe un caso de asistencia para los [ya migrados](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.

### Error de usuario Type2e {#type2e-user-failure}

_Causa raíz_: este error puede deberse a varios motivos en el servidor.

_Resoluciones_:

Antes de la migración: envíe un caso de asistencia para los [que aún no se han migrado](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Después de la migración: envíe un caso de asistencia para los [ya migrados](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.
