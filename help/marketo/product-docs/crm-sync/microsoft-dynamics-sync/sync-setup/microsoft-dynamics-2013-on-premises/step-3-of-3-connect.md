---
unique-page-id: 3571819
description: Paso 3 de 3 - Connect Marketing y Dynamics (On-premies 2013) - Documentos de marketing - Documentación del producto
title: Paso 3 de 3 - Connect Marketing y Dynamics (On-situ 2013)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# Paso 3 de 3: Connect Marketing y Dynamics (locales de 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

¡Bien! Hemos instalado la solución y configurado el usuario de sincronización. A continuación, debemos conectar Marketing y Dynamics.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Instalación de la solución de marketing en Dynamics (On-situ 2013)](step-1-of-3-install.md)
>* [Paso 2 de 3: Configuración del usuario de sincronización para Marketing (On-situ en 2013)](step-2-of-3-configure.md)

>



>[!NOTE]
>
>**Se requieren permisos de administración**

## Especifique la información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketing y haga clic en **Administración**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Seleccione **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Haga clic en **EDITAR** en el **paso 1: Introduzca las credenciales**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales son correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, tendrá que obtener una nueva suscripción de marketing.

1. Introduzca el **nombre de usuario**, la **contraseña** y la **dirección URL** de Microsoft Dynamics y, a continuación, haga clic en **GUARDAR**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >El nombre de usuario de Marketing debe coincidir con el nombre de usuario del usuario de sincronización en CRM. El formato puede ser [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#631610061123070c0e020a0d4d000c0e) o DOMINIO\usuario.

   >[!TIP]
   >
   >¿No conoce la dirección URL? Aquí le mostraremos cómo encontrar la URL [del servicio de organización de](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics.

## Seleccionar campos para sincronizar {#select-fields-to-sync}

Ahora necesitamos seleccionar los campos que queremos sincronizar.

1. Haga clic en **EDITAR **en el **paso 2: Seleccione Campos para sincronizar**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleccione los campos que desea sincronizar con el objeto de que estén preseleccionados. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que se sincronizarán con Marketing.

1. Vaya a Administración y seleccione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en detalles de sincronización de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **EDITAR **en el **paso 3: Habilitar sincronización**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización con Microsoft Dynamics o cuando introduzca personas o leads manualmente.

1. Lea todo en la ventana emergente, escriba su correo electrónico y haga clic en **INICIO SYNC**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La primera sincronización puede tardar unas horas. Una vez que haya terminado, recibirá una notificación por correo electrónico.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

¡Excelente trabajo! Acaba de liberar el poder de la sincronización bidireccional entre Marketing y Microsoft Dynamics. Si ha adquirido Marketo Sales Insight, puede ser más divertido:

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics 2013](../../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)

>



