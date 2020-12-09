---
unique-page-id: 2360366
description: Paso 3 de 3 -Connect Marketing y Salesforce (Enterprise/Unlimited) - Documentos de marketing - Documentación del producto
title: 'Paso 3 de 3: Connect Marketing y Salesforce (Enterprise/Unlimited)'
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Paso 3 de 3: Connect Marketing y Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

En este artículo, configurará Marketing para que se sincronice con la instancia de Salesforce configurada.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Añadir campos de marketing a Salesforce (Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para el marketing (Enterprise/Unlimited)](../../../../../product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) [](https://community.marketo.com/MarketoTutorial?id=kA250000000Kz5rCAC)

>



## Recuperar token de seguridad de usuario de sincronización {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si ya tiene el distintivo de seguridad, vaya directamente a Definir credenciales de usuario de sincronización y felicitaciones para la preparación.

1. Inicie sesión en Salesforce con el usuario de sincronización de marketing, haga clic en el nombre del usuario de sincronización y, a continuación, en **Mi configuración**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. En la búsqueda rápida, escriba &quot;restaurar&quot; y haga clic en **Restablecer mi token** de seguridad.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Haga clic en **Restablecer token** de seguridad.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   El token de seguridad se le enviará por correo electrónico.

## Definir credenciales de usuario de sincronización {#set-sync-user-credentials}

1. En Marketing, vaya a **Administrador**, seleccione **CRM** y haga clic en **Sincronizar con [Salesforce.com](http://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Asegúrese de [ocultar todos los campos que no necesite](../../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) en Marketing desde el usuario de sincronización antes de hacer clic en **Sincronizar campos**. Una vez que haga clic en Sincronizar campos, todos los campos que pueda ver el usuario se crearán en el Editor de forma permanente y no se podrán eliminar.

1. Introduzca las credenciales de usuario de sincronización de Salesforce creadas en la parte 2 de la configuración de Salesforce ([Professional](https://community.marketo.com/MarketoArticle?id=kA050000000LJ3QCAW), [Enterprise](https://community.marketo.com/MarketoArticle?id=kA050000000LIwKCAW)) y haga clic en **Sincronizar campos**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marque **Simulador para pruebas** si está sincronizando un Simulador para pruebas de marketing con un Simulador para pruebas de Salesforce.

1. Lea la advertencia y haga clic en **Confirmar credenciales**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si quieres ver las [asignaciones y personalizarlas](https://docs.marketo.com/display/public/DOCS/Edit+Initial+Field+Mappings), esta es tu única oportunidad para hacerlo. Una vez que haga clic en Inicio Salesforce Sync, ya estará listo.

## Inicio Salesforce Sync {#start-salesforce-sync}

1. Haga clic en **Inicio de sincronización** de Salesforce para iniciar la sincronización persistente de Marketing y Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de Salesforce o cuando introduzca leads manualmente.

1. Haga clic en **INICIO SINCRONIZACIÓN**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >El tiempo para completar la sincronización inicial varía según el tamaño y la complejidad de la base de datos.

## Verificar sincronización {#verify-sync}

Marketo proporciona mensajes de estado para la sincronización de Salesforce en el área Administración. Puede comprobar que la sincronización funciona correctamente siguiendo estos pasos.

1. En Marketing, haga clic en **Administración** y, a continuación, en **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. El estado de sincronización está visible en la esquina superior derecha. Mostrará uno de los tres mensajes: **Última sincronización**, **sincronización en curso** o **error**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Vaya, acabas de configurar una de las características más poderosas de Marketo, ve!

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Paso 1 de 3: Añadir campos de marketing a Salesforce (Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para el marketing (Enterprise/Unlimited)](step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Instalación del paquete de perspectiva de ventas de marketing en la AppExchange de Salesforce](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar la perspectiva de ventas de marketing en Salesforce Enterprise/Unlimited](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>* [Pasos opcionales](http://docs.marketo.com/display/docs/optional+steps)

>



