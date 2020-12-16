---
unique-page-id: 3571830
description: Paso 3 de 3 -Conectar Microsoft Dynamics con Marketing (en línea) - Documentos de marketing - Documentación del producto
title: 'Paso 3 de 3: Conectar Microsoft Dynamics con Marketing (en línea)'
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---


# Paso 3 de 3: Conectar Microsoft Dynamics con Marketing (en línea) {#step-of-connect-microsoft-dynamics-with-marketo-online}

Este es el último paso de la sincronización. ¡Ya casi llegamos!

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Instalación de la solución de marketing (en línea)](step-1-of-3-install.md)
   >
   >
* [Paso 2 de 3: Configurar usuario de sincronización de marketing en Dynamics](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Se requieren permisos de administración**

## Especifique la información del usuario de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Inicie sesión en Marketing y haga clic en **Administración**.

   ![](assets/login-admin.png)

1. Haga clic en **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Seleccione **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Haga clic en **Editar** en el **paso 1: Introduzca las credenciales**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Asegúrese de que sus credenciales son correctas, ya que no podemos revertir los cambios de esquema posteriores después del envío. Si se guardan credenciales incorrectas, tendrá que obtener una nueva suscripción de marketing.

1. Introduzca el **nombre de usuario**, la **contraseña** y la **dirección URL** de Microsoft Dynamics (el ID de cliente y el secreto de cliente son opcionales). Haga clic en **Guardar** cuando termine.

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >El nombre de usuario de Marketing debe coincidir con el nombre de usuario del usuario de sincronización en CRM. El formato puede ser [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#bcc9cfd9cefcd8d3d1ddd5d292dfd3d1) o DOMINIO\usuario.

## Seleccionar campos para sincronizar {#select-fields-to-sync}

1. Haga clic en **Editar** en el **paso 2: Seleccione Campos para sincronizar**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleccione los campos que desea sincronizar con el objeto de que estén preseleccionados. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## Sincronizar campos para un filtro personalizado {#sync-fields-for-a-custom-filter}

Si ha creado un filtro personalizado, asegúrese de entrar y seleccionar los nuevos campos que se sincronizarán con Marketing.

1. Vaya a Administración y seleccione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en detalles de sincronización de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Habilitar sincronización {#enable-sync}

1. Haga clic en **Editar** en el **paso 3: Habilitar sincronización**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización con Microsoft Dynamics o cuando introduzca personas o leads manualmente.

1. Lea todo lo que aparece en la ventana emergente, escriba su dirección de correo electrónico y haga clic en Sincronización de **Inicio**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La primera sincronización puede tardar unas horas. Una vez que haya terminado, recibirá una notificación por correo electrónico.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

¡Excelente trabajo!
