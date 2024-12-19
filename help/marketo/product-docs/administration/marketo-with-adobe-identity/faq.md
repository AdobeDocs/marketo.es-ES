---
description: Preguntas frecuentes sobre Adobe Identity Management - Documentos de Marketo - Documentación del producto
title: PREGUNTAS FRECUENTES SOBRE ADOBE IDENTITY MANAGEMENT
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: ec0fcba763a50348c3424a1ba33c5fc700093c68
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 0%

---

# PREGUNTAS FRECUENTES SOBRE ADOBE IDENTITY MANAGEMENT {#adobe-identity-management-faq}

**¿Qué es la identidad de Adobe?**

Adobe El sistema Identity Management consta de tres componentes.

* [!DNL Adobe Identity Service]: administra la autenticación y validación del usuario final, incluido el inicio de sesión único (SSO) de federación y tiempo de ejecución.

* Adobe Admin Console: El Admin Console proporciona una ubicación central para administrar los derechos de Adobe en toda la organización. Gestiona la administración de usuarios, el servicio en la nube, el derecho de licencia de escritorio y la configuración de federación, y proporciona funciones de seguridad para evitar la pérdida de datos.

* API de administración de usuarios de Adobe (UMAPI): permite a las organizaciones administrar usuarios y autorizaciones empresariales en Adobe Admin Console a nivel de API.

**¿Cuándo se integrarán las suscripciones de Marketo Engage existentes con IMS?**

Las suscripciones de Marketo Engage existentes se están migrando actualmente al IMS de Adobe en cualquier evento de ventas, que incluye renovaciones, eventos de recontratación o complementos. Las migraciones fuera de un evento de ventas ahora son compatibles desde octubre de 2024.

**Después de la migración, ¿seguirán siendo iguales las direcciones URL de los Marketo Engage?**

No. Las direcciones URL tendrán un aspecto diferente tras la migración.

**¿Hay algo que necesitemos hacer para prepararnos para el cambio de dirección URL?**

Sí. Después de la migración, Marketo Engage pasará de ser atendido desde experience.adobe.com a Adobe Experience Cloud. Deberá trabajar con su equipo de TI para realizar la lista de permitidos de todos los dominios de Adobe enumerados [ en la parte superior de este artículo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} a fin de evitar interrupciones en el acceso de los Marketo Engage.

Los vínculos y marcadores anteriores a los recursos de Marketo Engage en el dominio engage-xx.marketo.com _seguirán funcionando_. Sin embargo, primero debe iniciar sesión en la instancia de Marketo Engage de la dirección URL a la que está navegando. Por ejemplo, para navegar hasta un marcador de una campaña inteligente en una instancia con Munchkin ID 123-ABC-456, primero debe iniciar sesión en la instancia de Marketo Engage con Munchkin ID 123-ABC-456.

**¿Cuál es la diferencia entre un administrador de productos de Adobe y un administrador de Marketo Engage?**

* Adobe Product Admin es una nueva función de la plataforma de Marketo.
* La función Administrador de productos de Adobe se concede a los usuarios añadidos como administradores de productos en Adobe Admin Console
* Adobe Product Admin es una función de solo lectura y no se puede editar ni eliminar del Marketo Engage.
* El administrador de productos de Adobe tiene los mismos derechos y privilegios que un administrador de Marketo estándar.
* La función de administrador de Marketo Engage sigue siendo administrador y se concede a un usuario en Marketo Engage.

**¿Hay algún cambio en la compatibilidad con el cliente de la API de administración de usuarios?**

Sí. Aquellos que se hayan incorporado al IMS de Adobe no pueden utilizar todas las API de administración de usuarios de Marketo existentes. Para las acciones de invitación, actualización y eliminación de usuarios, se debe usar el Adobe [API de IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"}. Para la administración de funciones, las API de administración de usuarios de Marketo siguen aplicándose. Aparte de esto, no hay otros cambios en la compatibilidad con el cliente de la API de REST de Marketo.

**¿Con quién nos ponemos en contacto para obtener soporte si estamos integrados con IMS?**

* Migración previa al usuario: casos de compatibilidad de archivos en la [Comunidad de países de mercadotecnia](https://nation.marketo.com/t5/support/ct-p/Support) o el correo electrónico `customercare@marketo.com`.

* Migración posterior al usuario: casos de compatibilidad con archivos en la [Comunidad de países de mercadotecnia](https://nation.marketo.com/t5/support/ct-p/Support) o el correo electrónico `customercare@marketo.com`.

* Finalización de la migración posterior a la asistencia: los administradores de soporte técnico pueden archivar casos a través del Portal de soporte técnico para Experience League.

Si dispone de Ultimate Success, puede acceder al servicio de guante blanco de migración de Admin Console. Póngase en contacto con el equipo de la cuenta de Adobe (su administrador de cuentas) para obtener ayuda.

**Si uso una identidad de Adobe para acceder a otras aplicaciones de Adobe, ¿puedo usarla para acceder a Marketo?**

Aunque tenga otros productos de Adobe, no puede acceder a Marketo con identidad de Adobe hasta que se migre la suscripción a IMS.

**¿Los roles de usuario de Marketo (dentro de los espacios de trabajo) se administran en Adobe Admin Console?**

No. La administración de funciones de usuario (en espacios de trabajo) se completa en Marketo Engage.

**Soy administrador de Marketo con una suscripción integrada a IMS y no tengo acceso al Admin Console. ¿Cómo puedo obtener acceso?**

Cualquier administrador de sistemas de Adobe o de productos que tenga acceso al Admin Console de su organización podrá proporcionarle acceso. Si no está seguro de qué persona de su organización tiene privilegios de administrador en la consola, póngase en contacto con el [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**¿Cómo agregaría un administrador usuarios a Marketo [!DNL Sales Connect]?**

Aunque habrá una tarjeta de producto en el Admin Console para [!DNL Sales Connect], el Admin Console no debe usarse para agregar o administrar usuarios. El siguiente vínculo permitirá a los administradores administrar usuarios mediante Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**¿Dónde puedo obtener más información acerca de Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/es/enterprise/admin-guide.html){target="_blank"}.

**¿Debo ir a la sección Administración de Marketo para realizar cambios en la cuenta de usuario de mi cuenta?**

No, debe navegar a [account.adobe.com](https://account.adobe.com){target="_blank"}.

**¿Cómo funciona esto con el identificador universal de Marketo?**

Los usuarios incorporados a la identidad de Adobe pueden acceder fácilmente a todas las suscripciones habilitadas para IMS a través del conmutador de suscripciones del producto.

**¿Funciona esto con SSO?**

Sí. La integración de Marketo con Adobe IMS admite usuarios de ID universal y SSO. SSO ahora está dirigido por Adobe IMS y se configura en el nivel de organización en Adobe Admin Console. [Obtenga más información aquí](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

**Ya me he incorporado a Identidad de Adobe y ahora deseo implementar SSO. ¿Qué debo hacer?**

Si desea implementar el inicio de sesión único y su suscripción se ha incorporado a Adobe Identity sin SSO implementado en la organización de Adobe, envíe un ticket a [Soporte técnico de Marketo](https://nation.marketo.com/){target="_blank"} y especifique el tema como &quot;Marketo en Admin Console, implementación de SSO&quot;.

**¿Cómo funciona la autorización de dispositivos?**

Adobe IMS no admite nada como la función de autorización de dispositivos de Marketo.

**¿Todavía es posible usar la función &quot;Iniciar sesión en el cuadro de diálogo de usuario de invitación&quot; para que el inicio de sesión de un usuario sea único en su correo electrónico?**

No. El flujo de trabajo Invitación de usuario ya no está activo cuando una suscripción está habilitada para IMS, por lo que la función ya no es válida. La identidad de Adobe requiere que la identidad de un usuario esté impulsada por su correo electrónico.

**Para Adobe IMS, ¿tenemos la opción de usar Adobe ID, Enterprise ID o Federated ID?**

Sí, usted determina el tipo de identidad para que su organización la apoye. Encontrará más información aquí: [Información general de identidad](https://helpx.adobe.com/es/enterprise/using/identity.html) y aquí: [Configurar identidad](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html){target="_blank"}.

**¿Qué tarjetas de producto se admiten en Adobe Admin Console?**

Las tarjetas de producto admitidas son: Marketo Engage, Marketo Measure, Dynamic Chat de Marketo, Marketo Sales Connect y Acciones de perspectiva de ventas de Marketo.

**¿Qué sucede si mi inicio de sesión de usuario no coincide con mi correo electrónico cuando migre a una identidad de Adobe?**

Los usuarios actuales de Marketo Engage con inicios de sesión diferentes de su dirección de correo electrónico ya no iniciarán sesión con esa credencial una vez migrados a una identidad de Adobe. Las identidades de Adobe siempre se autentican con la dirección de correo electrónico de un usuario. Puede actualizar una dirección de correo electrónico de identidad de Adobe en [account.adobe.com](https://account.adobe.com){target="_blank"}.

**¿Qué sucede después de la migración de identidad de Adobe si mi suscripción utiliza la configuración de restricción de IP?**

Cuando las suscripciones se incorporan a Adobe Identity, la configuración de restricción de IP no se migra a Adobe Admin Console. La configuración de restricción de IP de Marketo incluye permitir solo acceso desde direcciones IP específicas y bloquear el acceso a direcciones IP específicas. En este momento, el sistema Identity Management de Adobe no admite funciones de restricción de IP.

A principios de 2025, Adobe Identity Management System lanzará una función para admitir que solo se permitan direcciones IP específicas, lo que admitirá una transición para los usuarios de Marketo que actualmente utilizan esta función. Los usuarios que actualmente utilicen esta función no se someterán a la migración de usuarios hasta que se publique la función. Una vez implementada la función, se notificará a los usuarios de la programación de su migración. Se proporcionará más información sobre la función cuando esté disponible.

Los usuarios que actualmente utilizan la restricción de IP, que bloquea el acceso a direcciones específicas, ya no podrán utilizar esta función después de migrarla a Adobe Identity, ya que no es compatible con Adobe Identity Management System.

**¿Qué sucede después de la migración de identidad de Adobe si tengo usuarios con un rol que tiene la opción de &#39;Omitir el inicio de sesión único&#39;?**

Cuando las suscripciones se incorporan a la identidad de Adobe, el inicio de sesión único (SSO) se configura en el nivel de organización de Adobe para todos los usuarios. Cuando se configura el SSO, se aplicará a todos los usuarios de Marketo o a todas las instancias de Marketo de esa organización de Adobe. Anteriormente, Marketo admitía permitir que una función de usuario se configurara para tener la opción de &#39;Omitir el inicio de sesión único&#39;. Adobe Identity Management System no lo admite.

**Tengo más de una suscripción, pero no todas tienen habilitado el inicio de sesión único. ¿Qué sucede después de la migración de identidad de Adobe?**

Cuando las suscripciones se incorporan a Adobe Identity, el inicio de sesión único (SSO) se configura en el nivel de organización de Adobe. Esto significa que el SSO se aplica a todas las instancias de producto de la organización de Adobe. Cuando se configura el SSO, se aplicará a todas las instancias de Marketo de esa organización de Adobe. Anteriormente, Marketo admitía esta configuración en el nivel de instancia. Esto no es compatible con el sistema Identity Management de Adobe.

**¿Se necesitan cambios en los CNAME, SPF o DKIM que usamos actualmente para Marketo Engage después de la migración de identidad de Adobe?**

No, estas configuraciones no se ven afectadas.

**¿Cómo puedo evitar que las sesiones agoten el tiempo de espera?**

En [Configuración avanzada](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings), puede personalizar la duración máxima de sesión deseada (se requieren permisos de administración del sistema). Se recomienda establecer esta configuración después de la migración del producto, pero antes de la migración del usuario.

**Ahora tengo que navegar al Experience Cloud para acceder al Marketo Engage. ¿Hay alguna manera de optimizar este flujo?**

Sí. Puede crear un marcador de explorador del vínculo que se inicia después de hacer clic en el botón **Iniciar** en la página de entrada de la instancia del Marketo Engage para omitir esa página en adelante.

![](assets/faq-1.png)
