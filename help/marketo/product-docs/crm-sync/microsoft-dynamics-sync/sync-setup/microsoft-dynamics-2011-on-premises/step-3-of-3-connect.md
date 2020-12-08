---
unique-page-id: 3571809
description: 'Paso 3 de 3: Conectar Microsoft Dynamics con Marketing (On-premies 2011) - Documentos de marketing - Documentación del producto'
title: 'Paso 3 de 3: Conectar Microsoft Dynamics con Marketing (On-situ 2011)'
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# Paso 3 de 3: Conectar Microsoft Dynamics con Marketing (On-situ 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

¡Bien! Hemos instalado la solución y configurado el usuario de sincronización. A continuación, debemos conectar Marketing y Dynamics.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Instalación de la solución de marketing (locales para 2011)](step-1-of-3-install.md)
>* [Paso 2 de 3: Configuración del usuario de sincronización de marketing en Dynamics (On-premies 2011)](step-2-of-3-set-up.md)


>[!NOTE]
>
>**Se requieren permisos de administración**

## Especifique la información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketing y haga clic en **Administración**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Haga clic en **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Haga clic en **Editar** en el **paso 1: Introduzca las credenciales.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales son correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, tendrá que obtener una nueva suscripción de marketing.

1. Introduzca el **nombre de usuario**, la **contraseña** y la **URL** de CRM y, a continuación, haga clic en **Guardar**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >El nombre de usuario de Marketing debe coincidir con el nombre de usuario del usuario de sincronización en CRM. El formato puede ser [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) o DOMINIO\usuario.

   >[!TIP]
   >
   >¿No conoce la dirección URL? Aquí le mostraremos cómo encontrar la URL [del servicio de organización de](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics.

## Seleccionar campos para sincronizar {#select-fields-to-sync}

Ahora necesitamos seleccionar los campos que queremos sincronizar.

1. Haga clic en **Editar** en **el paso 2: Seleccione Campos para sincronizar.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Hay campos preseleccionados que se sincronizarán. Añada más si lo desea y haga clic en **Guardar**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que se sincronizarán con Marketing.

1. Vaya a Administración y seleccione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en detalles de sincronización de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **Editar** en el **paso 3: Habilitar sincronización**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización con Microsoft Dynamics o cuando introduzca personas o leads manualmente.

1. Lea todo lo que aparece en la ventana emergente, escriba su correo electrónico y haga clic en Sincronización de **Inicio**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La primera sincronización puede tardar unas horas. Una vez que haya terminado, recibirá una notificación por correo electrónico.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   ¡Excelente trabajo!
