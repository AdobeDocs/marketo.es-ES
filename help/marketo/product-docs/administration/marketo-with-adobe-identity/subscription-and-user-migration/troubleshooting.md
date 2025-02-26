---
description: Guía de solución de problemas de IMS de Adobe - Documentos de Marketo - Documentación del producto
title: Guía de resolución de problemas de Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
source-git-commit: eccebb8352c56770dea5af9395c8bc83a08525dd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Guía de resolución de problemas de Adobe IMS {#adobe-ims-troubleshooting-guide}

Durante el proceso de migración de usuarios de IMS, se crea un usuario de Adobe para cada usuario de Marketo Engage que se migra. A veces, no se crea (por varios motivos, relacionados con el registro del usuario en Active Directory o problemas con la dirección de correo electrónico). Cuando esto sucede, el administrador de Marketo Engage ve las razones en el campo de estado de migración del usuario en la consola de migración automática. Consulte cómo resolver varios problemas de creación de usuarios de Adobe a continuación.

## Mensajes de error {#error-messages}

* <a href="#not-in-directory">No está en el directorio</a>
* <a href="#gmail-invalid-character">Carácter no válido de Gmail</a>
* <a href="#inactive-user">Usuario inactivo</a>
* <a href="#not-in-domain">No está en el dominio</a>
* <a href="#create-failure">Error al crear</a>
* <a href="#type2e-user-failure">Error de usuario Type2e</a>



<table>
<thead>
  <tr>
    <th style="width:20%">Mensaje de error</th>
    <th style="width:40%">Causa principal</th>
    <th style="width:40%">Resoluciones</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">No está en el directorio</a></i></td>
    <td>El usuario no existe en Active Directory (AD). Para cualquier organización con SSO que tenga habilitada la sincronización de AD, la creación de usuarios solo se permite mediante el proveedor de identidad (IdP). Por lo tanto, no se pudo agregar el usuario a través de Admin Console durante la migración de usuarios.</td>
    <td>Migrar: es necesario agregar al usuario a Active Directory con los permisos adecuados. Administrador de Marketo para volver a ejecutar la migración de este usuario desde la consola de migración. 
    <br>No migrar: el administrador de Marketo omitirá al usuario en la consola de migración. El botón "Migración completada" aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en él para concluir el proceso de migración de usuarios.</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Carácter no válido de Gmail</a></i></td>
    <td>Según la directiva de seguridad de Adobe, '.' Los signos "+" y "+" no se permiten solo en direcciones de correo electrónico de dominios de Gmail  
    <br>Se permiten ambos caracteres especiales en una dirección de correo electrónico de un dominio que no es Gmail. </td>
    <td>Migrar: la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir con la política de seguridad de Adobe. Administrador de Marketo para volver a ejecutar la migración de este usuario desde la consola de migración.<br>No migrar: el administrador de Marketo omitirá al usuario en la consola de migración. El botón "Migración completada" aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en él para concluir el proceso de migración de usuarios.</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">Usuario inactivo</a></i></td>
    <td>La sincronización de AD está habilitada y la cuenta federada del usuario existe pero en estado inactivo/deshabilitado.</td>
    <td>Migrar: es necesario restaurar el estado y los permisos adecuados del usuario. Administrador de Marketo para volver a ejecutar la migración de este usuario desde la consola de migración.
    <br>No migrar: el administrador de Marketo omitirá al usuario en la consola de migración. El botón "Migración completada" aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en él para concluir el proceso de migración de usuarios.</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">No está en el dominio</a></i></td>
    <td>La aplicación de dominios está habilitada en Admin Console, pero el dominio de la dirección de correo electrónico del usuario no es uno de los dominios permitidos. 
    <br>Las directivas de aplicación de dominio se establecen en el nivel de directorio.</td>
    <td>Migrar: la dirección de correo electrónico debe actualizarse en Marketo Engage para cumplir con la política de aplicación de dominios o el administrador del sistema puede <a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    mueva el dominio a otro directorio deshabilitado de aplicación de dominio (DE) </a>o <a href="https://helpx.adobe.com/es/enterprise/using/set-up-identity.html">cree un nuevo directorio</a> que no esté en la directiva DE. Administrador de Marketo para volver a ejecutar la migración de este usuario desde la consola de migración. <br>No migrar: el administrador de Marketo omitirá al usuario en la consola de migración. El botón "Migración completada" aparece cuando se contabilizan todos los usuarios migrando o omitiendo. Haga clic en él para concluir el proceso de migración de usuarios.</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">Error al crear</a></i></td>
    <td>Varias razones en el backend de.</td>
    <td>Envíe un caso de asistencia.</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Error de usuario Type2e</a></i></td>
    <td>Varias razones en el backend de.</td>
    <td>Envíe un caso de asistencia.</td>
  </tr>
</tbody>
</table>
