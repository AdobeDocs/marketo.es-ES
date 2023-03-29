---
unique-page-id: 2360366
description: 'Paso 3 de 3: Conexión de Marketo y Salesforce (Enterprise/Unlimited): Documentos de Marketo: Documentación del producto'
title: 'Paso 3 de 3: Conexión de Marketo y Salesforce (Enterprise/Unlimited)'
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '469'
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

1. Inicie sesión en Salesforce con el usuario de sincronización de Marketo, haga clic en el nombre del usuario de sincronización y, a continuación, **Mis ajustes**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. En la búsqueda rápida, escriba &quot;restablecer&quot; y haga clic en **Restablecer mi token de seguridad**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Haga clic en **Restablecer token de seguridad**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   El token de seguridad se le enviará por correo electrónico.

## Establecer credenciales de usuario de sincronización {#set-sync-user-credentials}

1. En Marketo, vaya a **Administrador**, seleccione **CRM** y haga clic en **Sincronizar con [Salesforce.com](https://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Asegúrese de [ocultar todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) en Marketo desde el usuario de sincronización antes de hacer clic en **Campos de sincronización**. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Introduzca las credenciales del usuario de sincronización de Salesforce creadas en la parte 2 de la configuración de Salesforce ([Profesional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) o [Empresa](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) y haga clic en **Campos de sincronización** (compruebe **Sandbox** solo si está sincronizando un Simulador para pruebas de Marketo con un Simulador para pruebas de Salesforce).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Si ve un botón &quot;Iniciar sesión en Salesforce&quot; en lugar de los campos Nombre de usuario/Contraseña/Token, su suscripción a Marketo está habilitada para OAuth. Por favor [consulte este artículo](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Tan pronto como la sincronización comience usando un conjunto de Credenciales, **no se puede cambiar las credenciales o la suscripción de Salesforce**. Si desea utilizar la autenticación básica, póngase en contacto con el equipo de cuentas de Adobe (su administrador de cuentas).

1. Lea la advertencia y haga clic en **Confirmar credenciales**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si desea ver el [asignaciones y personalizaciones](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)¡Esta es tu única oportunidad de hacerlo! Una vez que haga clic en Iniciar sincronización de Salesforce, se habrá completado.

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

1. En Marketo, haga clic en **Administrador**, luego **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. El estado de sincronización es visible en la esquina superior derecha. Muestra uno de los tres mensajes siguientes: **Última sincronización**, **Sincronización en curso** o **Error**.

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

