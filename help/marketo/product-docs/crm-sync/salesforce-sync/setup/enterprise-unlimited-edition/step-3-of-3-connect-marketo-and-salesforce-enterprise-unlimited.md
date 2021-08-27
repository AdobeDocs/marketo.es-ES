---
unique-page-id: 2360366
description: 'Paso 3 de 3: Conexión de Marketo y Salesforce (Enterprise/Unlimited): Documentos de Marketo: Documentación del producto'
title: 'Paso 3 de 3: Conexión de Marketo y Salesforce (Enterprise/Unlimited)'
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo y Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

En este artículo, configurará Marketo para que se sincronice con la instancia de Salesforce configurada.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## Recuperar el token de seguridad del usuario de sincronización {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si ya tiene el token de seguridad, proceda directamente a Sincronizar credenciales de usuario y felicitaciones para su preparación.

1. Inicie sesión en Salesforce con el usuario de sincronización de Marketo, haga clic en el nombre del usuario de sincronización y, a continuación, haga clic en **My Settings**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. En la búsqueda rápida, escriba &quot;reset&quot; y haga clic en **Reset My Security Token**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Haga clic en **Restablecer token de seguridad**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   El token de seguridad se le enviará por correo electrónico.

## Establecer credenciales de usuario de sincronización {#set-sync-user-credentials}

1. En Marketo, vaya a **Admin**, seleccione **CRM** y haga clic en **Sincronizar con [Salesforce.com](https://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Asegúrese de [ocultar todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) en Marketo del usuario de sincronización antes de hacer clic en **Sincronizar campos**. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Introduzca las credenciales de usuario de sincronización de Salesforce creadas en la parte 2 de la configuración de Salesforce ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) o [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) y haga clic en **Campos de sincronización** (marque **Simulador para pruebas** solo si está sincronizando un Simulador para pruebas de Marketo con un Simulador para pruebas de Salesforce).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Si ve un botón &quot;Iniciar sesión en Salesforce&quot; en lugar de los campos Nombre de usuario/Contraseña/Token, su suscripción a Marketo está habilitada para OAuth. Por favor [consulte este artículo](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Tan pronto como la sincronización empieza a utilizar un conjunto de Credenciales, **no hay cambio de las credenciales de Salesforce o la suscripción**. Si desea utilizar la autenticación básica, póngase en contacto con el gestor de éxito del cliente.

1. Lea la advertencia y haga clic en **Confirmar credenciales**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si desea ver los [mappings y personalizarlos](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), esta es su única oportunidad para hacerlo. Una vez que haga clic en Iniciar sincronización de Salesforce, se habrá completado.

## Iniciar sincronización de Salesforce {#start-salesforce-sync}

1. Haga clic en **Iniciar sincronización de Salesforce** para iniciar la sincronización persistente de Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente con una sincronización de Salesforce o cuando introduzca posibles clientes manualmente.

1. Haga clic en **Iniciar sincronización**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >El tiempo para completar la sincronización inicial varía según el tamaño y la complejidad de la base de datos.

## Verificar sincronización {#verify-sync}

Marketo proporciona mensajes de estado para la sincronización de Salesforce en el área de administración. Puede verificar que la sincronización funciona correctamente siguiendo estos pasos.

1. En Marketo, haga clic en **Admin** y, a continuación, en **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. El estado de sincronización es visible en la esquina superior derecha. Muestra uno de los tres mensajes siguientes: **Última sincronización**, **Sincronización en curso** o **Fallido**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Vaya, acaba de terminar de configurar una de las funciones más poderosas de Marketo, ¡vaya!

>[!MORELIKETHIS]
>
>* [Paso 1 de 3: Agregar campos de Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Instalación del paquete de perspectivas de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

