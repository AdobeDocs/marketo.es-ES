---
description: 'Explicación de la suscripción de Marketo y la migración de usuarios a Adobe Admin Console: documentos de Marketo, documentación del producto'
title: Explicación de la suscripción de Marketo y la migración de usuarios a Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 0%

---

# Explicación de la suscripción de Marketo y la migración de usuarios a Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

El Adobe está mejorando la forma de administrar las suscripciones y los usuarios de Adobe Marketo Engage, lo que aumenta la productividad para usted y su organización. Como parte de este cambio, el Adobe de está migrando las suscripciones de Marketo Engage y los usuarios a Adobe Admin Console. Se trata de una migración necesaria que no afecta a ningún flujo de trabajo, contenido, integración o recurso de marketing.

Descubra cómo puede utilizar Adobe Admin Console para administrar sus derechos de Adobe en toda la organización con [Guía de administración de Enterprise y equipos](https://helpx.adobe.com/es/enterprise/admin-guide.html){target="_blank"}.

## ¿Qué está cambiando? {#what-is-changing}

Como parte de la migración, la suscripción y la administración de usuarios se moverán de la aplicación de Marketo al Adobe Admin Console.

* **Los administradores del sistema administrarán las suscripciones en Adobe Admin Console**. Ver todos los productos de Adobe en una sola consola.

* **Los administradores de productos administrarán los usuarios y su acceso en Adobe Admin Console**. Añada y elimine usuarios para todas sus suscripciones de Adobe.

* **Los usuarios iniciarán sesión con la identidad de Adobe**. El Adobe migrará a los usuarios existentes a Adobe Admin Console. Los usuarios iniciarán sesión en sus suscripciones de Marketo con su nueva identidad de Adobe: un Federated ID de Adobe ID o de Adobe (SSO).

* **No hay cambios en la forma de administrar el resto de las funciones** dentro de la propia aplicación de Marketo Engage, incluida la administración de funciones, funciones de usuario, espacios de trabajo, funcionalidad y comportamiento.

## Cronología del Recorrido de migración {#migration-journey-timeline}

El Adobe migrará primero sus suscripciones de Marketo Engage a Adobe Admin Console y, a continuación, migrará todos los usuarios existentes con direcciones de correo electrónico comprobadas. Si es administrador del sistema o de productos de Marketo, recibirá correos electrónicos que le guiarán a través del recorrido de migración. Esta es una cronología de lo que puede esperar:

### Migración de suscripción completa {#subscription-migration-complete}

Los administradores del sistema recibirán un correo electrónico cuando se complete la migración de suscripción a Adobe Admin Console.

Es posible que los administradores del sistema tengan que completar algunos pasos necesarios antes de que comience la migración de usuarios para minimizar el impacto a los usuarios de Marketo:

* Si los usuarios de Marketo inician sesión con SSO, deberá configurarlo en Adobe Admin Console para que puedan seguir iniciando sesión con SSO. Si los usuarios de Marketo no utilizan actualmente el SSO, pero desea configurarlo en Adobe Admin Console, puede hacerlo en este punto del recorrido de migración.

* Si ya administra otros productos de Adobe en su Adobe Admin Console, es posible que Adobe solicite su consentimiento para migrar automáticamente a los usuarios a la consola existente. Haga clic en el botón &quot;Comenzar&quot; del correo electrónico para ir a la página de consentimiento.

No hay cambios en la administración de usuarios en este momento. Aunque los productos de Marketo aparecen en el Admin Console, los administradores de Marketo seguirán administrando a los usuarios en el área de administración de Marketo y los usuarios seguirán iniciando sesión con su Marketo Identity hasta que se complete la migración de usuarios. Durante este tiempo, los productos de Marketo no se pueden administrar en Admin Console hasta que comience la migración de usuarios. Esto incluye la instancia de Dynamic Chat asociada con la suscripción.

>[!NOTE]
>
>Si actualmente no utiliza el SSO, pero está pensando en implementarlo, le sugerimos que lo haga antes de que se produzca la migración de usuarios. Si desea implementar el inicio de sesión único y su suscripción se ha incorporado a Adobe Identity sin SSO implementado en la organización de Adobe, envíe un ticket a [Asistencia de Marketo](https://nation.marketo.com/){target="_blank"} y especifique el tema como &quot;Marketo en Admin Console, implementación de SSO&quot;.

### Programar migración de usuarios {#schedule-user-migration}

Una vez que el administrador del sistema complete los requisitos previos descritos en la sección anterior, el Adobe programará automáticamente la migración de usuario con 30 días de antelación y se comunicará con los administradores de productos de Marketo para administrar la migración de usuario.

Los administradores de productos de Marketo:

* Reciba un correo electrónico con la fecha de inicio de la migración de usuarios programada con 30 días de antelación.

* Obtenga acceso a la consola de migración de Marketo, ubicada en el área de administración de Marketo, donde tiene la opción de cambiar la fecha de migración de una suscripción.

>[!NOTE]
>
>Debido a la complejidad de la migración, los cambios de fecha están restringidos a no más de 30 días después de la fecha programada. Envíe un correo electrónico a `marketocares@marketo.com` si necesita una fecha posterior.

* Consulte un titular en Mi Marketo que muestra una cuenta atrás para la fecha de inicio de la migración de usuarios.

* Reciba un correo electrónico recordatorio el día anterior a la fecha de inicio de la migración de usuarios.

### Preparar usuarios para el día de la migración {#prepare-users-for-migration-day}

Como administrador de productos de Marketo, se le recomienda asegurarse de que todos los usuarios estén preparados para el día de la migración.

* Marque [verificación por correo electrónico](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} estado para todos los usuarios en el área de administración de Marketo. Anime a los usuarios que no hayan verificado su dirección de correo electrónico a que lo hagan y ayude a los usuarios a resolver cualquier desafío al completar el proceso de verificación.

* Prepare a todos los usuarios para la próxima migración a la identidad de Adobe.

>[!NOTE]
>
>A medida que los usuarios migren, recibirán un correo electrónico del Adobe de notificándoles el cambio en la forma en que inician sesión en Marketo. Se invitará a los usuarios a aceptar una invitación para iniciar sesión con ID de Adobe por primera vez, ya sea iniciando sesión con un Adobe ID existente o configurando uno nuevo con la misma dirección de correo electrónico.

>[!IMPORTANT]
>
>Si un usuario Marketo Engage no comprueba su dirección de correo electrónico, no se migra a una Adobe ID y pierde el acceso a la suscripción de Marketo una vez completada la migración de la suscripción. Para recuperar el acceso, un administrador de productos de Marketo tendría que agregarlos como un nuevo usuario.

### Qué esperar el día de la migración {#what-to-expect-on-migration-day}

Todas las suscripciones de Marketo con una zona horaria de EE. UU. se migrarán a partir de la medianoche (hora estándar del Pacífico) de la fecha de inicio de la migración. La migración de usuarios para todas las demás suscripciones comenzará a medianoche del huso horario especificado de la suscripción.

**El Adobe migrará automáticamente primero a los administradores de Marketo**. Cuando se migran administradores de Marketo a Identidad de Adobe, se les asigna la función Administrador de productos de Adobe dentro de la aplicación de Marketo junto con cualquier otra función que tuvieran anteriormente.

**Si su suscripción a Marketo tiene menos de 75 usuarios**, el Adobe migrará automáticamente al resto de los usuarios. Este flujo de trabajo tiene como objetivo ofrecer el máximo nivel de automatización para minimizar la sobrecarga para los usuarios de Marketo de Adobe. No se requiere ninguna acción por su parte para ejecutar la migración.

**Si su suscripción a Marketo tiene más de 75 usuarios**, los administradores de productos de Marketo tendrán acceso al área de migración de usuarios de autoservicio de la consola de migración de Marketo, que se encuentra en el área de administración de Marketo. Para aquellos que necesiten un mayor control durante el proceso de migración de usuarios, los administradores de productos de Marketo podrán empezar a seleccionar usuarios para migrar en lotes o en cualquier momento. Una vez seleccionados los usuarios, los administradores tienen la opción de &quot;Migrar ahora&quot; o &quot;Programar migración&quot; para una fecha posterior, lo que proporciona a los administradores la flexibilidad y el control definitivos sobre los usuarios que se migrarán cuando.

>[!NOTE]
>
>No se perderá el acceso al producto durante la migración de usuarios. Si un usuario ha iniciado sesión durante el tiempo en el que se está migrando su usuario, se cerrará la sesión del usuario y se le pedirá que vuelva a iniciarla en cuestión de minutos mediante Identidad de Adobe una vez completada la migración.

A medida que los usuarios migren, recibirán un correo electrónico de Adobe notificándoles el cambio en la forma en que inician sesión en Marketo. Se invitará a los usuarios a aceptar una invitación para iniciar sesión con Adobe Identity por primera vez, ya sea iniciando sesión con un Adobe ID existente o configurando un nuevo Adobe ID con la misma dirección de correo electrónico.

Encontrará más información en [Inicio de sesión de usuario con Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} and [Adobe Identity Management FAQ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migración de usuarios completada {#user-migration-complete}

Adobe notificará por correo electrónico a todos los administradores del sistema y de productos cuando se hayan migrado todos los administradores y usuarios. En este momento, todos los usuarios de Marketo para esa suscripción iniciarán sesión en Marketo con ID de Adobe y los administradores de productos solo administrarán usuarios en Adobe Admin Console.

## Obtener asistencia {#get-support}

Para obtener asistencia adicional relacionada con su suscripción o migración de usuarios, envíe un correo electrónico a `marketocares@marketo.com`.
