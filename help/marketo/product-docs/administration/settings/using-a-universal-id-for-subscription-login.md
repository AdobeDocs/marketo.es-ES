---
unique-page-id: 10100311
description: Uso de un ID universal para el inicio de sesión de Suscripción - Documentos de marketing - Documentación del producto
title: Uso de un ID universal para el inicio de sesión de Suscripción
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Uso de un ID universal para el inicio de sesión de Suscripción {#using-a-universal-id-for-subscription-login}

Un ID universal permite acceder a varias suscripciones de marketing con un solo inicio de sesión y cambiar rápidamente de una suscripción a otra. Sin embargo, puede utilizar distintos inicios de sesión para sus suscripciones si lo desea.

Con el ID universal, sigue creando tickets de asistencia para cada una de sus suscripciones individuales.

Se respetan los ajustes del nivel de suscripción para los usuarios que utilizan el identificador universal, por ejemplo, funciones, permisos y políticas de contraseña. Los cambios en el nivel de perfil del usuario se reflejan en todas las suscripciones, por ejemplo, el nombre, los apellidos y la dirección de correo electrónico.

## Configuración de un identificador universal {#setting-up-a-universal-id}

Desde cada instancia individual, el administrador de marketing debe invitarlo a cada una de sus diferentes suscripciones con el mismo inicio de sesión. Marketing no puede combinar automáticamente los inicios de sesión existentes. Una vez que habilite el ID universal, **la instancia de Marketing no estará disponible** durante un máximo de 30 minutos. Si tiene una base de usuarios más grande, podría ser un poco más larga.

>[!CAUTION]
>
>Si el ID único o el ID universal están activados para un usuario, sus funciones y espacios de trabajo pueden **no** editarse tras su configuración inicial.

>[!NOTE]
>
>Si tiene varios ID de inicio de sesión de suscripción, también puede tener varios perfiles de comunidad. Asegúrese de elegir el ID de su ID universal que está conectado al perfil que desea utilizar, y esto es para la instancia de producción, no para el simulador para pruebas.

## Inicio de sesión {#logging-in}

Al iniciar sesión para aceptar una invitación a una segunda suscripción con un ID universal, verá la página de inicio de sesión de la opción de inclusión. Aquí debe marcar una casilla de verificación para aceptar los términos y condiciones. Una vez que haya aceptado, verá la página de restablecimiento normal, no esta, para los inicios de sesión posteriores. Al aceptar los términos y condiciones, está permitiendo a Marketing distribuir los datos básicos de perfil (como el nombre, los apellidos y la dirección de correo electrónico) a los centros de datos en diferentes ubicaciones en las que se aloja la suscripción.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>Los ID que ya no utilice permanecen a menos que el administrador de suscripciones los elimine. Le recomendamos que las mantenga, por ejemplo, si tiene un informe privado, asignado a usted mismo, al que solo se pueda acceder con esa ID. En este caso, tiene sentido mover estos informes privados a su nuevo ID universal y, a continuación, eliminar el ID existente.

## Contraseñas {#passwords}

Con el ID universal para varias suscripciones, Marketing aplica automáticamente la política de contraseñas más estricta. Por ejemplo, si algunas suscripciones requieren una longitud mínima de contraseña y otras no, la longitud mínima se aplicará a todas las suscripciones.

Con un ID universal para varias suscripciones, solo usted puede cambiar la contraseña.

>[!NOTE]
>
>Marketo pedirá a los usuarios que deseen utilizar el identificador universal que restablezcan su contraseña si la contraseña de la suscripción actual no cumple la política de contraseñas de la segunda suscripción a la que se les invita.

## Cambio entre Suscripciones {#switching-between-subscriptions}

Con un ID universal, puede ver la suscripción en la que ha iniciado sesión y seleccionar otras suscripciones a las que tiene acceso de inicio de sesión. En la mayoría de los casos, puede cambiar entre ellos sin tener que cerrar la sesión ni volver a iniciarla.

![](assets/image2016-11-3-15-3a10-3a16.png)

Al cerrar sesión y volver a iniciarla, Marketing inicia sesión automáticamente en la suscripción en la que inició sesión por última vez. Luego puede cambiar a una suscripción diferente si es necesario.

## Perfiles de la comunidad {#community-profiles}

Si tiene varias suscripciones, puede tener varios perfiles de comunidad. Le recomendamos que elija el inicio de sesión vinculado a su perfil de comunidad más activo.

## Plataforma móvil {#mobile-platform}

Los usuarios con ID universal pueden ver sus datos en Momentos de marketing y en la aplicación de registro de evento para iPad desde la suscripción en la que iniciaron sesión por última vez. No puede cambiar suscripciones desde la propia plataforma móvil.

