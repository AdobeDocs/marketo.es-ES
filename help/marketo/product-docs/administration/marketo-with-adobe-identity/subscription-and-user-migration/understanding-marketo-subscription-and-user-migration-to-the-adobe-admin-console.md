---
description: Cambios cuando las suscripciones y los usuarios migran a Adobe Admin Console, incluidas las funciones de administrador del sistema y administrador de productos, inicio de sesión con Adobe Identity, direcciones URL y cronología de la migración.
title: Explicación de la suscripción de Marketo y la migración de usuarios a Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 98%

---

# Explicación de la suscripción de Marketo y la migración de usuarios a Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe está mejorando la forma de administrar las suscripciones y los usuarios de Adobe Marketo Engage, ofreciéndoles una mayor productividad a usted y su organización. Como parte de este cambio, Adobe está migrando sus suscripciones y usuarios de Marketo Engage a Adobe Admin Console. Se trata de una migración necesaria que no afecta a ningún flujo de trabajo de marketing, contenido, integraciones o recursos.

>[!TIP]
>
>Aprenda a utilizar Adobe Admin Console para administrar sus derechos de Adobe en toda la organización con la [Guía de administración para empresas y equipos](https://helpx.adobe.com/es/enterprise/admin-guide.html){target="_blank"}.

## ¿Qué cambios hay? {#what-is-changing}

Como parte de la migración, la suscripción y la administración de usuarios se moverán de la aplicación de Marketo a Adobe Admin Console.

* **Los administradores del sistema administrarán las suscripciones en Adobe Admin Console**. Vea todos sus productos de Adobe en una sola consola.

* **Los administradores de productos administrarán a los usuarios y su acceso en Adobe Admin Console**. Añada y quite usuarios en todas sus suscripciones de Adobe. Adobe Admin Console no admite la caducidad del acceso basado en usuarios. Los usuarios con acceso a Marketo Engage programado para caducar después de la migración migran igualmente y se les concede acceso que no caduca. Después de la migración, deberán eliminarse manualmente en la fecha de vencimiento deseada (o antes).

* **Los usuarios iniciarán sesión con Adobe Identity**. Adobe migrará los usuarios existentes a Adobe Admin Console. Los usuarios iniciarán sesión en sus suscripciones de Marketo con su nueva identidad de Adobe, ya sea Adobe ID o Adobe Federated ID (SSO).

* **El aspecto de las direcciones URL será diferente después de la migración**. Marketo Engage pasará de estar disponible desde experience.adobe.com a Adobe Experience Cloud, y las URL estarán en el siguiente formato: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (las XXX representan el ID de Munchkin y la parte @tenantID corresponde a su organización de Adobe). Deberá trabajar con su equipo de TI para incluir en la lista de permitidos todos los dominios de Adobe enumerados [en la parte superior de este artículo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} a fin de evitar interrupciones en el acceso a Marketo Engage.

Los números de ID de los recursos siguen siendo los mismos. Y los vínculos y marcadores anteriores a los recursos de Marketo Engage en el dominio engage-xx.marketo.com _seguirán funcionando_. Sin embargo, primero debe iniciar sesión en la instancia de Marketo Engage para la URL a la que vaya a navegar. Por ejemplo, para navegar a un marcador de una campaña inteligente en una instancia con el ID de Munchkin 123-ABC-456, primero debe iniciar sesión en la instancia de Marketo Engage con el ID de Munchkin 123-ABC-456.

Si bien aún no se ha planificado, el trabajo de desarrollo futuro puede interrumpir esta función de redireccionamiento. Para evitar interrupciones inesperadas, se recomienda actualizar los marcadores lo antes posible.

## ¿Qué es lo que no cambia? {#what-is-not-changing}

* **No hay cambios en la forma de administrar todas las demás funcionalidades** dentro de la propia aplicación de Marketo Engage, incluida la administración de características, funciones de usuario, espacios de trabajo, funcionalidades y comportamientos. La administración de usuarios locales (solo API) permanece en la pestaña _Usuarios y funciones_ del área de administración de Marketo.

## Cronología del recorrido de migración {#migration-journey-timeline}

Adobe migrará primero las suscripciones de Marketo Engage a Adobe Admin Console y, a continuación, migrará todos los usuarios existentes con direcciones de correo electrónico verificadas. Si es usted administrador del sistema o administrador de productos de Marketo, recibirá correos electrónicos que le guiarán a través del recorrido de la migración. Aquí puede ver una cronología con lo que cabe esperar:

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### Migración de suscripción completada {#subscription-migration-complete}

Los administradores del sistema recibirán un correo electrónico cuando se complete la migración de suscripción a Adobe Admin Console.

Es posible que los administradores del sistema tengan que completar algunos pasos obligatorios antes de que comience la migración de usuarios para minimizar el impacto para los usuarios de Marketo.

* Si los usuarios de Marketo actualmente inician su sesión con SSO, deberá configurar el SSO en Adobe Admin Console para que los usuarios puedan seguir iniciando sesión con SSO. Si los usuarios de Marketo no utilizan actualmente el SSO, pero desea configurarlo en Adobe Admin Console, puede hacerlo en este momento del recorrido de migración.

* Si ya administra otros productos en Adobe Admin Console, Adobe puede solicitar su consentimiento para migrar automáticamente los usuarios a la consola existente. Haga clic en el botón “Empezar” del correo electrónico para ir a la página de consentimiento.

No hay cambios en la administración de usuarios en este momento. Aunque los productos de Marketo aparecen en Admin Console, los administradores de Marketo seguirán administrando a los usuarios en el área de administración de Marketo y los usuarios seguirán iniciando sesión con su identidad de Marketo hasta que se complete la migración de usuarios. Durante este tiempo, los productos de Marketo no se pueden administrar en Admin Console hasta que comience la migración de usuarios. Esto incluye la instancia de Dynamic Chat asociada con la suscripción.

>[!NOTE]
>
>Si actualmente no utiliza el SSO, pero está pensando en implementarlo, le sugerimos que lo haga antes de que se realice la migración de usuarios. Si desea implementar el inicio de sesión único y su suscripción se ha incorporado a Adobe Identity sin SSO implementado en la organización de Adobe, envíe una solicitud de asistencia al [Soporte técnico de Marketo](https://nation.marketo.com/){target="_blank"} y especifique el tema como “Marketo en Admin Console, implementación de SSO”.

### Programar migración de usuarios {#schedule-user-migration}

Una vez que el administrador del sistema complete los requisitos previos descritos en la sección anterior, Adobe programará automáticamente la migración de usuarios con 30 días de antelación y se comunicará con los administradores de productos de Marketo para administrar la migración de usuarios.

Los administradores de productos de Marketo tendrán los siguientes beneficios:

* Recibirán con 30 días de antelación un correo electrónico indicándoles la fecha de inicio programada para la migración de usuarios.

* Obtendrán acceso a la Consola de migración de Marketo, ubicada en el área de administración de Marketo, donde tienen la opción de cambiar la fecha de migración de una suscripción.

>[!NOTE]
>
>Debido a la complejidad de la migración, los cambios de fecha están restringidos a no más de 30 días después de la fecha programada. Envíe un correo electrónico a `marketocares@marketo.com` si necesita una fecha posterior.

* Verán un banner en Mi Marketo que muestra la cuenta atrás hasta la fecha de inicio de la migración de usuarios.

* Recibirán un correo electrónico recordatorio el día anterior a la fecha de inicio de la migración de usuarios.

### Preparar usuarios para el día de la migración {#prepare-users-for-migration-day}

Como administrador de productos de Marketo, se le recomienda asegurarse de que todos los usuarios estén preparados para el día de la migración.

* Compruebe el estado de [verificación de, correo electrónico](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} para todos los usuarios en el área de administración de Marketo. Anime a los usuarios que no hayan verificado su dirección de correo electrónico a que lo hagan, ayude a los usuarios a resolver cualquier reto que se les presente mientras completan el proceso de verificación.

* Busque en la bandeja de entrada de correo electrónico las notificaciones de los usuarios “bloqueados”. Aconseje a los usuarios que hayan sido bloqueados que restablezcan su contraseña para volver a tener acceso a Marketo Engage antes del día de la migración.

* Prepare a todos los usuarios para la próxima migración a Adobe Identity.

>[!IMPORTANT]
>
>Si un usuario de Marketo Engage no verifica su dirección de correo electrónico o se encuentra bloqueado en el momento de la migración de usuarios, no se migrará a un Adobe ID y perderá el acceso a la suscripción de Marketo una vez completada la migración de la suscripción. Para recuperar el acceso, un administrador de productos de Marketo tendría que añadirlos como nuevos usuarios.

### Qué cabe esperar el día de la migración {#what-to-expect-on-migration-day}

Todas las suscripciones de Marketo con zona horaria en EE. UU. se migrarán a partir de la medianoche (hora estándar del Pacífico) de la fecha de inicio de la migración. La migración de usuarios para todas las demás suscripciones comenzará a medianoche de la zona horaria especificada para la suscripción.

**Adobe migrará automáticamente primero a los administradores de Marketo (con función de administrador estándar)**. Cuando los administradores de Marketo se migren a Adobe Identity con una función de administrador de productos de Admin Console, se les asignará la función de administrador de productos de Adobe dentro de la aplicación Marketo, junto con cualquier otra funciónque tuvieran anteriormente.

**Si su suscripción a Marketo no tiene SSO en Marketo o en su organización de Adobe**, Adobe migrará automáticamente al resto de los usuarios. Este flujo de trabajo tiene como objetivo ofrecer el máximo nivel de automatización para minimizar la sobrecarga para los usuarios de Adobe Marketo. No se requiere ninguna acción por su parte para ejecutar la migración.

**Si su suscripción a Marketo tiene SSO en Marketo o en su organización de Adobe**, los administradores de Marketo tendrán acceso al área de migración de usuarios de autoservicio de la Consola de migración de Marketo, que se encuentra en el área de administración de Marketo. Para aquellos que necesiten un mayor control durante el proceso de migración de usuarios, los administradores de Marketo podrán empezar a seleccionar los usuarios para su migración por lotes o todos al mismo tiempo. Una vez seleccionados los usuarios, los administradores tienen la opción de “Migrar ahora” o “Programar migración” para una fecha posterior, lo que proporciona a los administradores la flexibilidad y el control definitivos sobre qué usuarios se van a migrar y cuándo.

>[!NOTE]
>
>No se perderá el acceso al producto durante la migración de usuarios. Si un usuario ha iniciado sesión durante el tiempo en el que se está migrando su usuario, se cerrará la sesión del usuario y el sistema le indicará que vuelva a intentar iniciar sesión en unos minutos mediante Adobe Identity, una vez ya completada la migración. El usuario debe aceptar la invitación haciendo clic en el vínculo del correo electrónico de asignación de derechos que se envía cuando la migración de usuarios se ha realizado correctamente.

Cuando se migra a los usuarios, estos recibirán un correo electrónico de Adobe donde se les notifica el cambio en la forma en que inician sesión en Marketo. Los usuarios **deben** aceptar una invitación para iniciar sesión con Adobe Identity por primera vez, ya sea iniciando sesión con un Adobe ID existente o configurando un nuevo Adobe ID con la misma dirección de correo electrónico.

Puede encontrar más información en [Migración a Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [Inicio de sesión del usuario con Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} y [Preguntas frecuentes sobre Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migración de usuarios completada {#user-migration-complete}

Adobe enviará una notificación por correo electrónico a todos los administradores de sistema y administradores de productos cuando se hayan migrado todos los administradores y usuarios. En ese momento, todos los usuarios de Marketo de esa suscripción iniciarán sesión en Marketo mediante Adobe Identity y los administradores de productos solo administrarán usuarios en Adobe Admin Console.

## Obtener ayuda {#get-support}

Para obtener ayuda adicional sobre su suscripción o migración de usuario, envíe un correo electrónico a `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Información general sobre la migración a Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Inicio de sesión de usuario con Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Preguntas frecuentes sobre Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [Tutorial de migración a Adobe Identity Management](https://experienceleague.adobe.com/es/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
