---
description: 'Información general de Adobe Identity Management: documentos de Marketo, documentación del producto'
title: Información general sobre Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# Información general sobre Adobe Identity Management {#adobe-identity-management-overview}

Si tiene una cuenta nueva con Adobe Marketo Engage (cuenta nueva, no solo una nueva para una cuenta existente) a partir del 15 de febrero de 2022, puede que se integre con el sistema Identity Management de Adobe, según el paquete de producto comprado. Para saber si lo tiene, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas).

Las suscripciones de Marketo existentes empezarán a migrarse al sistema Identity Management de Adobe en el segundo semestre de 2023.

>[!NOTE]
>
>El Soporte de Marketo no podrá proporcionar ninguna actualización con respecto a la migración de IMS de Adobe. El equipo de cuenta de Adobe se pondrá en contacto con el calendario estimado en los próximos meses.

## Niveles de perfil {#profile-levels}

Las suscripciones de Adobe Marketo Engage integradas en el sistema Identity Management de Adobe admiten varios perfiles. A continuación se indican los tipos de perfiles de usuario relevantes para esta integración.

<table>
 <tr>
  <td><strong>Administrador del sistema de Adobe Admin Console</strong></td>
  <td>Responsable de configurar los conceptos de identidad de la organización de Adobe y del producto de Marketo Engage en Adobe Admin Console. Se ha concedido la función en la configuración de organización de Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrador de productos Adobe Admin Console</strong></td>
  <td>Responsable de otorgar derechos a los usuarios para el producto de Marketo Engage en Adobe Admin Console. Función otorgada en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrador de perfil de producto de Adobe Admin Console</strong></td>
  <td>Responsable de la administración de usuarios dentro de un perfil de producto. No pueden administrar usuarios que no pertenezcan a ese perfil específico. Un administrador de perfil de producto no tiene acceso a la aplicación de Marketo a menos que se añada al perfil de producto como usuario. Su función seguiría siendo un usuario estándar (espacio de trabajo predeterminado si tiene más de un espacio de trabajo).
</td>
 </tr>
 <tr>
  <td><strong>Administrador de productos de Marketo Engage</strong></td>
  <td>Una persona a la que se le ha dado acceso a un Marketo Engage con privilegios administrativos. Se ha concedido la función en Marketo Engage, no en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Usuario Marketo Engage</strong></td>
  <td>Una persona a la que se le ha dado acceso al Marketo Engage. Sin privilegios administrativos.</td>
 </tr>
</table>

## Preguntas frecuentes {#faq}

**¿Qué es la identidad de Adobe?**

Adobe El sistema Identity Management consta de tres componentes.

* [!DNL Adobe Identity Service]: administra la autenticación y validación del usuario final, incluido el inicio de sesión único (SSO) de federación y tiempo de ejecución.

* Adobe Admin Console: El Admin Console proporciona una ubicación central para administrar los derechos de Adobe en toda la organización. Gestiona la administración de usuarios, el servicio en la nube, el derecho de licencia de escritorio y la configuración de federación, y proporciona funciones de seguridad para evitar la pérdida de datos.

* API de administración de usuarios de Adobe (UMAPI): permite a las organizaciones administrar usuarios y autorizaciones empresariales en Adobe Admin Console a nivel de API.

**¿Cuándo se integrarán las suscripciones de Marketo Engage existentes con IMS?**

Las suscripciones de Marketo existentes se migrarán al sistema Identity Management de Adobe a finales de este año. El Soporte de Marketo no podrá proporcionar ninguna actualización con respecto a la migración de IMS de Adobe. El equipo de cuenta de Adobe se pondrá en contacto con el calendario estimado en los próximos meses.

**¿Cuál es la diferencia entre un administrador de productos de Adobe y un administrador de Marketo Engage?**

* Adobe Product Admin es una nueva función de la plataforma de Marketo.
* La función Administrador de productos de Adobe se concede a los usuarios añadidos como administradores de productos en Adobe Admin Console
* Adobe Product Admin es una función de solo lectura y no se puede editar ni eliminar del Marketo Engage.
* El administrador de productos de Adobe tiene los mismos derechos y privilegios que un administrador de Marketo estándar.
* La función de administrador de Marketo Engage sigue siendo administrador y se concede a un usuario en Marketo Engage.

**¿Hay algún cambio en la compatibilidad con el cliente de la API de User Management?**

Sí. Aquellos que se hayan incorporado al IMS de Adobe no pueden utilizar todas las API de administración de usuarios de Marketo existentes. Para las acciones de invitación, actualización y eliminación de usuarios, el Adobe [API de IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} debe usarse. Para la administración de funciones, las API de administración de usuarios de Marketo siguen aplicándose. Aparte de esto, no hay otros cambios en la compatibilidad con el cliente de la API de REST de Marketo.

**¿Con quién nos ponemos en contacto para obtener asistencia si estamos integrados con IMS?**

Debe seguir el procedimiento estándar de contacto [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**Si utilizo una identidad de Adobe para acceder a otras aplicaciones de Adobe, ¿puedo utilizarla para acceder a Marketo?**

Aunque tenga otros productos de Adobe, no puede acceder a Marketo con identidad de Adobe hasta que se migre la suscripción a IMS.

**¿Las funciones de usuario de Marketo (dentro de los espacios de trabajo) se administran en Adobe Admin Console?**

No. La administración de funciones de usuario (en espacios de trabajo) se completa en Marketo Engage.

**Soy administrador de Marketo con una suscripción integrada de IMS y no tengo acceso al Admin Console. ¿Cómo puedo obtener acceso?**

Cualquier administrador de sistemas de Adobe o de productos que tenga acceso al Admin Console de su organización podrá proporcionarle acceso. Si no está seguro de qué persona de su organización tiene privilegios de administrador en la consola, póngase en contacto con [Adobe del Servicio de atención al cliente](https://helpx.adobe.com/contact.html){target="_blank"}.

**¿Cómo agregaría un administrador usuarios a Marketo? [!DNL Sales Connect]?**

Mientras que habrá una tarjeta de producto en Admin Console para [!DNL Sales Connect], el Admin Console no debe utilizarse para añadir o administrar usuarios. El siguiente vínculo permite a los administradores administrar usuarios mediante Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**¿Dónde puedo obtener más información sobre Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

**¿Sigo yendo a la sección Administración en Marketo para realizar cambios en la cuenta de usuario de mi cuenta?**

No, tendría que navegar a [account.adobe.com](https://account.adobe.com){target="_blank"}.

**¿Cómo funciona esto con el ID universal de Marketo?**

Los usuarios incorporados a la identidad de Adobe pueden acceder fácilmente a todas las suscripciones habilitadas para IMS a través del conmutador de suscripciones del producto.

**¿Funciona con SSO?**

Sí. La integración de Marketo con Adobe IMS admite usuarios de ID universal y SSO. SSO ahora está dirigido por Adobe IMS y se configura en el nivel de organización en Adobe Admin Console. [Obtenga más información aquí](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**¿Cómo funciona la autorización de dispositivos?**

Adobe IMS no admite nada como la función de autorización de dispositivos de Marketo.

**¿Sigue siendo posible utilizar la función &quot;Iniciar sesión en el cuadro de diálogo de usuario de invitación&quot; para que el inicio de sesión de un usuario sea único desde su correo electrónico?**

No. El flujo de trabajo Invitación de usuario ya no está activo cuando una suscripción está habilitada para IMS, por lo que la función ya no es válida. La identidad de Adobe requiere que la identidad de un usuario esté impulsada por su correo electrónico.

**Para Adobe IMS, ¿tenemos la opción de usar Adobe ID, Enterprise ID o Federated ID?**

Sí, usted determina el tipo de identidad para que su organización la apoye. Puede encontrar más información aquí: [Información general de identidad](https://helpx.adobe.com/enterprise/using/identity.html) y aquí: [Configurar identidad](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**¿Qué tarjetas de producto se admiten en Adobe Admin Console?**

Las tarjetas de producto admitidas son: Marketo Engage, Marketo Measure, Dynamic Chat de Marketo, Marketo Sales Connect y Acciones de perspectiva de ventas de Marketo.

>[!MORELIKETHIS]
>
>* [Ajustes de administración](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Agregar o quitar un administrador de productos](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Agregar o quitar un usuario](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
