---
description: 'Información general: Documentos de Marketo: Documentación del producto'
title: Resumen
hide: true
hidefromtoc: true
source-git-commit: 6047665cf94a4b212734667feeb5fce911ffdebb
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Resumen {#overview}

Si la suscripción al Marketo Engage de Adobe se ha aprovisionado el 21/10/4 o después, se integra con el sistema Identity Management de Adobe. AIMS permite a los usuarios iniciar sesión en aplicaciones de Marketo Engage y otras aplicaciones de Experience Cloud mediante una identidad de Adobe común.

## Niveles de perfil

Hay tres niveles de perfil.

<table>
 <tr>
  <td><strong>Administrador del sistema</strong></td>
  <td>Responsable de la configuración de conceptos de identidad para la organización de Adobe y el producto Marketo Engage en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrador de productos</strong></td>
  <td>Responsable de autorizar a los usuarios para el producto Marketo Engage en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Usuario</strong></td>
  <td>Una persona a la que se ha dado acceso al Marketo Engage. Sin privilegios administrativos.</td>
 </tr>
</table>

## Preguntas frecuentes

**¿Qué es la identidad de Adobe?**

El sistema Identity Management de Adobe consta de tres componentes.

* Servicio de identidad de Adobe: Gestiona la autenticación y validación del usuario final, incluida la federación y el inicio de sesión único (SSO) en tiempo de ejecución.

* Adobe Admin Console: El Admin Console proporciona una ubicación central para administrar las autorizaciones de Adobe en toda la organización. Gestiona la administración de usuarios, el servicio en la nube, la asignación de licencias de escritorio, la configuración de federación y proporciona funciones de seguridad para la prevención de pérdidas de datos.

* API de administración de usuarios de Adobe (UMAPI): Permite a las organizaciones administrar usuarios y autorizaciones empresariales en Adobe Admin Console a nivel de API.

**¿Cuál es la diferencia entre un administrador de productos de Adobe y un administrador Marketo Engage?**

* El administrador de productos de Adobe es una función nueva en la plataforma de Marketo.
* Es una función de solo lectura y no se puede editar ni eliminar de Marketo.
* Tiene los mismos derechos y privilegios que el administrador estándar de Marketo.

**¿Se ha producido algún cambio en la compatibilidad con el cliente de API?**

Sí. Aquellos que se hayan incorporado a Adobe IMS no podrán utilizar las API de administración de usuarios de Marketo existentes. Utilizarían el [API de IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html).

**¿Con quién nos ponemos en contacto para obtener asistencia?**

Seguiría el procedimiento estándar para ponerse en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

**¿Las funciones de usuario de Marketo (dentro de los espacios de trabajo) se administran en Adobe Admin Console?**

No. La administración de funciones de usuario (dentro de espacios de trabajo) se completa en Marketo.

**Soy administrador de Marketo y no tengo acceso al Admin Console. ¿Cómo obtengo acceso?**

Cualquier administrador de sistemas o productos que tenga acceso al Admin Console de su organización puede proporcionarle acceso. Si no está seguro de quién cuenta con privilegios de administrador en la consola, póngase en contacto con [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html).

**¿Cómo agregaría un administrador usuarios a Marketo Sales Connect?**

Aunque habrá una tarjeta de producto en AC for Sales Connect, AC no debe usarse para agregar/administrar usuarios. El siguiente vínculo permite a los administradores administrar usuarios mediante Marketo Sales Connect: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**¿Dónde puedo obtener más información sobre Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**¿Sigo yendo a la sección Administración de Marketo para realizar cambios en la cuenta?**

No, necesitaría navegar a [account.adobe.com](https://account.adobe.com).

**¿Cómo funciona esto con el ID universal de Marketo?**

Los usuarios incorporados a la identidad de Adobe pueden acceder a todas las suscripciones habilitadas para IMS sin problemas a través del conmutador de suscripciones del producto.

**¿Funciona con SSO?**

Sí. La integración de Marketo con Adobe IMS es compatible con los usuarios de ID universales y SSO. Ahora, SSO es impulsado por Adobe IMS y se configura en el nivel de organización en Adobe Admin Console. [Obtenga más información aquí](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**¿Cómo funciona la autorización de dispositivos?**

Actualmente, Adobe IMS no admite nada parecido a la función de autorización de dispositivos de Marketo.

**¿Todavía es posible utilizar la función &quot;Iniciar sesión en el diálogo de invitación de usuario&quot; para que el inicio de sesión sea único desde nuestro correo electrónico?**

No. El flujo de trabajo de invitación del usuario ya no está activo cuando una suscripción está habilitada para IMS, por lo que la función ya no es válida. La identidad de Adobe requiere que la identidad de un usuario se guíe por su correo electrónico.

**Para Adobe IMS, ¿tenemos la opción de usar Adobe ID, Enterprise ID o Federated ID?**

Sí, usted determina el tipo de identidad para que su organización sea compatible. Más información [here](https://helpx.adobe.com/enterprise/using/identity.html) y [here](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Configuración de administración](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Agregar o eliminar un administrador de productos](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Agregar o eliminar un usuario](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

