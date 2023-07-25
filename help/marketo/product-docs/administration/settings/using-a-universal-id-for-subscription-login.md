---
unique-page-id: 10100311
description: Uso de un ID universal para el inicio de sesión con suscripción - Documentos de Marketo - Documentación del producto
title: Uso de un ID universal para el inicio de sesión con suscripción
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Uso de un ID universal para el inicio de sesión con suscripción {#using-a-universal-id-for-subscription-login}

Un ID universal le permite acceder a varias suscripciones de Marketo con un solo inicio de sesión y cambiar entre suscripciones rápidamente. Sin embargo, puede utilizar diferentes inicios de sesión para sus suscripciones si lo desea.

Con el ID universal, sigue creando vales de soporte para cada una de sus suscripciones individuales.

La configuración del nivel de suscripción se respeta para los usuarios que utilizan un identificador universal como, por ejemplo, funciones, permisos y directivas de contraseña. Los cambios en el nivel de perfil del usuario se reflejan en todas las suscripciones, por ejemplo, nombre, apellidos y dirección de correo electrónico.

## Configuración de un ID universal {#setting-up-a-universal-id}

Todas las suscripciones a Marketo incluyen la función de ID universal opcional. Desde cada instancia individual, el administrador de Marketo debe invitarle a cada una de sus diferentes suscripciones con el mismo inicio de sesión. Marketo no puede combinar automáticamente los inicios de sesión existentes.

>[!NOTE]
>
>Si tiene varios ID de inicio de sesión con suscripción, también puede tener varios perfiles de comunidad. Asegúrese de elegir el ID del ID universal conectado al perfil que desea utilizar y que sea para la instancia de producción, no para la zona protegida.

## Iniciando sesión {#logging-in}

Cuando inicie sesión para aceptar una invitación a una segunda suscripción con un ID universal, verá la página de inicio de sesión de inclusión. En este caso, debe marcar una casilla de verificación para aceptar los términos y condiciones. Después de aceptar, verá la página de restablecimiento normal, no esta, para los inicios de sesión posteriores. Al aceptar los términos y condiciones, permite a Marketo distribuir los datos básicos del perfil (como el nombre, apellidos y dirección de correo electrónico) a los centros de datos de diferentes ubicaciones en las que se aloja la suscripción.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>Los ID que ya no utilice permanecerán a menos que el administrador de suscripciones los elimine. Le recomendamos que los conserve, en caso de que, por ejemplo, tenga un informe privado, asignado a usted mismo, al que solo se pueda acceder mediante ese ID. En este caso, tiene sentido mover estos informes privados a su nuevo ID universal y, a continuación, eliminar su ID existente.

## Contraseñas {#passwords}

Con el ID universal para varias suscripciones, Marketo aplica automáticamente la política de contraseñas más estricta. Por ejemplo, si algunas suscripciones requieren una longitud mínima de la contraseña y otras no, la longitud mínima se aplicará a todas las suscripciones.

Con un ID universal para varias suscripciones, solo usted puede cambiar la contraseña.

>[!NOTE]
>
>Marketo solicitará a los usuarios que deseen utilizar el ID universal que restablezcan su contraseña si la contraseña de la suscripción actual no cumple la política de contraseñas de la segunda suscripción a la que están siendo invitados.

## Cambio entre suscripciones {#switching-between-subscriptions}

Con un ID universal, puede ver la suscripción en la que ha iniciado sesión y seleccionar otras suscripciones a las que tiene acceso de inicio de sesión. En la mayoría de los casos, puede cambiar entre ellos sin tener que cerrar la sesión y volver a iniciarla.

![](assets/image2016-11-3-15-3a10-3a16.png)

Cuando cierra la sesión y vuelve a iniciarla, Marketo inicia sesión automáticamente en la suscripción en la que inició sesión por última vez. A continuación, puede cambiar a una suscripción diferente si es necesario.

## Perfiles de comunidad {#community-profiles}

Si tiene varias suscripciones, puede tener varios perfiles de la comunidad. Le recomendamos que elija el inicio de sesión vinculado a su perfil de comunidad más activo.

## Plataforma móvil {#mobile-platform}

Los usuarios con ID universal pueden ver sus datos en Momentos de Marketo y en la aplicación de registro de eventos de iPad desde la última suscripción en la que iniciaron sesión. Las suscripciones no se pueden cambiar desde la propia plataforma móvil.

>[!MORELIKETHIS]
>
>* [Agregar el inicio de sesión único a un portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Restringir el inicio de sesión del usuario a solo SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Invitación de usuarios de Marketo a dos instancias con ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
