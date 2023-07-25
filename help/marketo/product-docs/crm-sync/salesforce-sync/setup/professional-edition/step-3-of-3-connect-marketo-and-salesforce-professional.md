---
unique-page-id: 3571800
description: 'Paso 3 de 3: Conexión de Marketo y Salesforce (profesional): Documentos de Marketo: documentación del producto'
title: 'Paso 3 de 3: Conexión de Marketo y Salesforce (profesional)'
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo y Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

En este artículo, configurará Marketo para que se sincronice con la instancia de Salesforce configurada.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Agregar campos de Marketo a Salesforce (profesional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (profesional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

## Recuperar token de seguridad de usuario de sincronización {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si ya tiene el token de seguridad, vaya directamente a Establecer credenciales de usuario de sincronización y felicitaciones para la preparación.

1. Inicie sesión en Salesforce con el usuario de sincronización de Marketo, haga clic en el nombre del usuario de sincronización y luego **Mis configuraciones**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. En la barra de búsqueda de navegación, escriba &quot;restablecer&quot; y haga clic en **Restablecer mi token de seguridad**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Clic **Restablecer token de seguridad**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   El token de seguridad se le enviará por correo electrónico.

## Establecer credenciales de usuario de sincronización {#set-sync-user-credentials}

1. En Marketo, vaya a **Administrador**, seleccione **CRM** y haga clic en **Sincronizar con [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Asegúrese de [oculte todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) en Marketo desde el usuario de sincronización antes de hacer clic en **Sincronizar campos**. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Introduzca las credenciales del usuario de sincronización de Salesforce creadas en la parte 2 de la configuración de Salesforce ([Profesional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Empresa](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) y haga clic en **Sincronizar campos**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marque **Sandbox** si sincroniza una zona protegida de Marketo con una de Salesforce.

1. Lea la advertencia y haga clic en **Confirmar credenciales**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si desea ver el [asignaciones y personalizarlas](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)¡Esta es tu única oportunidad de hacerlo! Una vez que haga clic en Iniciar sincronización de Salesforce, ya estará listo.

## Iniciar sincronización de Salesforce {#start-salesforce-sync}

1. Clic **Iniciar sincronización de Salesforce** para iniciar la sincronización persistente entre Marketo y Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de Salesforce o cuando introduzca manualmente posibles clientes.

1. Clic **Iniciar sincronización**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >El tiempo para completar la sincronización inicial varía según el tamaño y la complejidad de la base de datos.

## Verificar sincronización {#verify-sync}

Marketo proporciona mensajes de estado para la sincronización de Salesforce en el área de Administración. Puede comprobar que la sincronización funciona correctamente siguiendo estos pasos.

1. En Marketo, haga clic en **Administrador**, entonces **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. El estado de sincronización es visible en la esquina superior derecha. Mostrará uno de los tres mensajes siguientes: **Última sincronización**, **Sincronización en curso**, o **Error**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

¡Vaya! Acaba de configurar una de las funciones más potentes de Marketo. ¡Ya está!

>[!MORELIKETHIS]
>
>* [Instalación del paquete de información de ventas de Marketo en la AppExchange de Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configuración de Marketo Sales Insight en Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
