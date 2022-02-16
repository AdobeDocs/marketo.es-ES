---
description: 'Información general: Documentos de Marketo: Documentación del producto'
title: Resumen
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 7eff888c0fdebf31da4706f70d1e99e8327807ca
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Resumen {#overview}

Si tiene una nueva cuenta con el Marketo Engage de Adobe (nueva cuenta, no solo una nueva instancia para una cuenta existente) a partir del 15 de febrero de 2022, puede integrarse con el sistema Identity Management de Adobe, según el paquete de productos comprado. Para averiguar si lo tiene, póngase en contacto con el administrador de Marketo o con el administrador de éxito del cliente de su cuenta.

Las suscripciones existentes a Marketo se migrarán a Adobe Identity Management System a partir de este año.

>[!NOTE]
>
>La asistencia de Marketo no podrá proporcionar ninguna actualización con respecto a la migración de IMS de Adobe. El Administrador de éxito de los clientes establecerá un plazo estimado para los próximos meses.

## Niveles de perfil

Las suscripciones del Marketo Engage de Adobe incorporadas al sistema Identity Management de Adobe admiten varios perfiles. Los siguientes son los tipos de perfiles de usuario relevantes en esta integración.

<table>
 <tr>
  <td><strong>Administrador del sistema de Adobe Admin Console</strong></td>
  <td>Responsable de la configuración de conceptos de identidad para la organización de Adobe y el producto Marketo Engage en Adobe Admin Console. Se concede la función en la configuración de la organización de Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrador de productos de Adobe Admin Console</strong></td>
  <td>Responsable de autorizar a los usuarios para el producto Marketo Engage en Adobe Admin Console. Se ha concedido la función en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrador del producto del Marketo Engage</strong></td>
  <td>Una persona a la que se ha dado acceso a un Marketo Engage con privilegios administrativos. Se concede la función de Marketo Engage, no de Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Usuario Marketo Engage</strong></td>
  <td>Una persona a la que se ha dado acceso al Marketo Engage. Sin privilegios administrativos.</td>
 </tr>
</table>

## Preguntas frecuentes

**¿Qué es la identidad de Adobe?**

El sistema Identity Management de Adobe consta de tres componentes.

* Servicio de identidad de Adobe: Gestiona la autenticación y validación del usuario final, incluida la federación y el inicio de sesión único (SSO) en tiempo de ejecución.

* Adobe Admin Console: El Admin Console proporciona una ubicación central para administrar las autorizaciones de Adobe en toda la organización. Gestiona la administración de usuarios, el servicio en la nube, la asignación de licencias de escritorio, la configuración de federación y proporciona funciones de seguridad para la prevención de pérdidas de datos.

* API de administración de usuarios de Adobe (UMAPI): Permite a las organizaciones administrar usuarios y autorizaciones empresariales en Adobe Admin Console a nivel de API.

**¿Cuándo se integrarán las suscripciones de Marketo Engage existentes con IMS?**

Las suscripciones de Marketo existentes se migrarán a Adobe Identity Management System más adelante este año. La asistencia de Marketo no podrá proporcionar ninguna actualización con respecto a la migración de IMS de Adobe. El Administrador de éxito de los clientes establecerá un plazo estimado para los próximos meses.

**¿Cuál es la diferencia entre un administrador de productos de Adobe y un administrador Marketo Engage?**

* El administrador de productos de Adobe es una función nueva en la plataforma de Marketo.
* El rol de administrador de productos de Adobe se concede a los usuarios agregados como administradores de productos en Adobe Admin Console
* El administrador de productos de Adobe es una función de solo lectura que no se puede editar ni eliminar del Marketo Engage.
* El administrador de productos de Adobe tiene los mismos derechos y privilegios que un administrador de Marketo estándar.
* La función de administrador Marketo Engage sigue siendo administrador y se concede a un usuario en Marketo Engage.

**¿Se ha producido algún cambio en la compatibilidad con el cliente de la API de administración de usuarios?**

Sí. Aquellos que se hayan incorporado a Adobe IMS no podrán utilizar todas las API de administración de usuarios de Marketo existentes. Para las acciones de invitación, actualización y eliminación del usuario, el Adobe [API de IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html) debe usarse. Para la administración de funciones, se siguen aplicando las API de administración de usuarios de Marketo. Aparte de esto, no hay otros cambios en la compatibilidad con el cliente de la API de REST de Marketo.

**¿Con quién nos ponemos en contacto si estamos integrados con IMS?**

Seguiría el procedimiento estándar para ponerse en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

**¿Las funciones de usuario de Marketo (dentro de los espacios de trabajo) se administran en Adobe Admin Console?**

No. La administración de funciones de usuario (dentro de espacios de trabajo) se completa en Marketo Engage.

**Soy administrador de Marketo en una suscripción integrada a IMS y no tengo acceso al Admin Console. ¿Cómo obtengo acceso?**

Cualquier administrador de sistemas de Adobe o de productos que tenga acceso al Admin Console de su organización podrá proporcionarle acceso. Si no está seguro de quién cuenta con privilegios de administrador en la consola, póngase en contacto con [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html).

**¿Cómo agregaría un administrador usuarios a Marketo Sales Connect?**

Aunque habrá una tarjeta de producto en Admin Console para Conexión de Ventas, el Admin Console no debe utilizarse para agregar o administrar usuarios. El siguiente vínculo permite a los administradores administrar usuarios mediante Marketo Sales Connect: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**¿Dónde puedo obtener más información sobre Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**¿Todavía accedo a la sección Administración de Marketo para realizar cambios en la cuenta de usuario de mi cuenta?**

No, necesitaría navegar a [account.adobe.com](https://account.adobe.com).

**¿Cómo funciona esto con el ID universal de Marketo?**

Los usuarios incorporados a la identidad de Adobe pueden acceder a todas las suscripciones habilitadas para IMS sin problemas a través del conmutador de suscripciones del producto.

**¿Funciona con SSO?**

Sí. La integración de Marketo con Adobe IMS es compatible con los usuarios de ID universales y SSO. Ahora, SSO es impulsado por Adobe IMS y se configura en el nivel de organización en Adobe Admin Console. [Obtenga más información aquí](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**¿Cómo funciona la autorización de dispositivos?**

Actualmente, Adobe IMS no admite nada parecido a la función de autorización de dispositivos de Marketo.

**¿Sigue siendo posible utilizar la función &quot;Iniciar sesión en el diálogo de invitación de usuario&quot; para que el inicio de sesión de un usuario sea único desde su correo electrónico?**

No. El flujo de trabajo de invitación del usuario ya no está activo cuando una suscripción está habilitada para IMS, por lo que la función ya no es válida. La identidad de Adobe requiere que la identidad de un usuario se guíe por su correo electrónico.

**Para Adobe IMS, ¿tenemos la opción de usar Adobe ID, Enterprise ID o Federated ID?**

Sí, usted determina el tipo de identidad para que su organización sea compatible. Puede encontrar más información aquí: [Información general sobre identidad](https://helpx.adobe.com/enterprise/using/identity.html) y aquí: [Configuración de identidad](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Configuración de administración](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Agregar o eliminar un administrador de productos](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Agregar o eliminar un usuario](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

