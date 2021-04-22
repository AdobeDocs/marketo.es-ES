---
unique-page-id: 10100311
description: 'Uso de un ID universal para el inicio de sesión de suscripción: Documentos de Marketo: Documentación del producto'
title: Uso de un ID universal para el inicio de sesión de suscripción
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Uso de un ID universal para el inicio de sesión de suscripción {#using-a-universal-id-for-subscription-login}

Un ID universal le permite acceder a varias suscripciones a Marketo con un solo inicio de sesión y cambiar rápidamente entre suscripciones. Sin embargo, si lo desea, puede usar distintos inicios de sesión para sus suscripciones.

Con el ID universal, seguirá creando tickets de asistencia para cada una de sus suscripciones individuales.

La configuración del nivel de suscripción se acepta para los usuarios que utilicen un ID universal, por ejemplo, funciones, permisos y políticas de contraseña. Los cambios en el nivel de perfil del usuario se reflejan en todas las suscripciones, por ejemplo, el nombre, los apellidos y la dirección de correo electrónico.

## Configuración de un identificador universal {#setting-up-a-universal-id}

Desde cada instancia individual, el administrador de Marketo debe invitarlo a cada una de las distintas suscripciones con el mismo inicio de sesión. Marketo no puede combinar automáticamente los inicios de sesión existentes. Una vez que habilite el ID universal, **la instancia de Marketo no estará disponible** durante un máximo de 30 minutos. Si tiene una base de usuarios más grande, podría ser un poco más larga.

>[!CAUTION]
>
>Si el ID único o el ID universal están habilitados para un usuario, sus funciones y espacios de trabajo **no** se pueden editar después de su configuración inicial.

>[!NOTE]
>
>Si tiene varios ID de inicio de sesión de suscripción, también puede tener varios perfiles de comunidad. Asegúrese de elegir el ID del ID universal que está conectado al perfil que desea utilizar, y eso es para la instancia de producción, no para el simulador para pruebas.

## Inicio de sesión {#logging-in}

Cuando inicie sesión para aceptar una invitación a una segunda suscripción mediante un ID universal, verá la página de inicio de sesión de inclusión. Aquí debe marcar una casilla de verificación para aceptar los términos y condiciones. Cuando haya aceptado, verá la página de restablecimiento normal, no esta, para los inicios de sesión posteriores. Al aceptar los términos y las condiciones, se permite a Marketo distribuir los datos básicos de perfil (como el nombre, los apellidos y la dirección de correo electrónico) a los centros de datos en diferentes ubicaciones en las que se aloja la suscripción.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>Los ID que ya no utilice permanecen a menos que el administrador de suscripciones los elimine. Le recomendamos que los mantenga, en caso de que, por ejemplo, tenga un informe privado, asignado a usted mismo, al que solo se pueda acceder mediante ese ID. En este caso, tiene sentido mover estos informes privados a su nuevo ID universal y, a continuación, eliminar el ID existente.

## Contraseñas {#passwords}

Con el ID universal para varias suscripciones, Marketo aplica automáticamente la política de contraseñas más estricta. Por ejemplo, si algunas suscripciones requieren una longitud mínima de la contraseña y otras no, la longitud mínima se aplicará a todas las suscripciones.

Con un ID universal para varias suscripciones, solo usted puede cambiar la contraseña.

>[!NOTE]
>
>Marketo pedirá a los usuarios que deseen utilizar el identificador universal que restablezcan su contraseña si la contraseña de la suscripción actual no cumple la política de contraseñas de la segunda suscripción a la que están invitados.

## Cambio entre suscripciones {#switching-between-subscriptions}

Con un ID universal, puede ver la suscripción en la que ha iniciado sesión y seleccionar otras suscripciones a las que tiene acceso de inicio de sesión. En la mayoría de los casos, puede cambiar entre ellos sin tener que cerrar la sesión y volver a iniciarla.

![](assets/image2016-11-3-15-3a10-3a16.png)

Al cerrar la sesión y volver a iniciarla, Marketo inicia sesión automáticamente en la suscripción en la que inició sesión por última vez. A continuación, puede cambiar a una suscripción diferente si es necesario.

## Perfiles de la comunidad {#community-profiles}

Si tiene varias suscripciones, puede tener varios perfiles de comunidad. Le recomendamos que elija el inicio de sesión vinculado a su perfil de comunidad más activo.

## Plataforma móvil {#mobile-platform}

Los usuarios con ID universal pueden ver sus datos en Marketo Moments y en la aplicación de registro de eventos de iPad desde la suscripción en la que iniciaron sesión por última vez. No puede cambiar las suscripciones desde la propia plataforma móvil.

>[!MORELIKETHIS]
>
>* [Agregar el inicio de sesión único a un portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Restringir el inicio de sesión del usuario solo a SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Invitación de usuarios de Marketo a dos instancias con ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

