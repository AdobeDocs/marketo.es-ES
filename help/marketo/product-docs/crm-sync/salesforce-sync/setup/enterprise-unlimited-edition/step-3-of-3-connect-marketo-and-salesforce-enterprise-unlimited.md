---
unique-page-id: 2360366
description: 'Paso 3 de 3: Conexión de Marketo y Salesforce (Enterprise/Unlimited), documentación de Marketo: documentación del producto'
title: 'Paso 3 de 3: Conexión de Marketo y Salesforce (empresarial/ilimitada)'
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: f27e0d42161161347cc4c774853fb04e7ccecb5c
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo y [!DNL Salesforce] (empresa/ilimitado) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

En este artículo, configurará Marketo para que se sincronice con la instancia [!DNL Salesforce] configurada.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Agregar campos de Marketo a [!DNL Salesforce] (Empresa/ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un [!DNL Salesforce] usuario para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

## Recuperar token de seguridad de usuario de sincronización {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si ya tiene el token de seguridad, vaya directamente a Establecer credenciales de usuario de sincronización y felicitaciones para la preparación.

1. Inicie sesión en [!DNL Salesforce] con el usuario de sincronización de Marketo, haga clic en el nombre del usuario de sincronización y, a continuación, en **[!UICONTROL Mi configuración]**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. En la búsqueda rápida, escriba &quot;restablecer&quot; y haga clic en **[!UICONTROL Restablecer mi token de seguridad]**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Haga clic en **[!UICONTROL Restablecer token de seguridad]**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   El token de seguridad se le enviará por correo electrónico.

## Establecer credenciales de usuario de sincronización {#set-sync-user-credentials}

1. En Marketo, ve a **[!UICONTROL Admin]**, selecciona **CRM** y haz clic en **[!UICONTROL Sincronizar con Salesforce.com]**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Asegúrese de [ocultar todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) en Marketo del usuario de sincronización antes de hacer clic en **[!UICONTROL Campos de sincronización]**. Una vez que haga clic en [!UICONTROL Sincronizar campos], todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Introduzca las credenciales de usuario de sincronización [!DNL Salesforce] creadas en la parte 2 de la configuración de [!DNL Salesforce] ([Profesional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) o [Empresa](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) y haga clic en **[!UICONTROL Campos de sincronización]** (marque **[!UICONTROL Zona protegida]** solo si está sincronizando una Zona protegida de Marketo con una de [!DNL Salesforce]).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Si ve el botón &quot;Iniciar sesión en [!DNL Salesforce]&quot; en lugar de los campos Nombre de usuario/Contraseña/Token, su suscripción a Marketo estará habilitada para OAuth. [Consulte este artículo](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Tan pronto como la sincronización comience a usar un conjunto de credenciales, **no hay cambio de credenciales o suscripción de [!DNL Salesforce]**. Si desea utilizar la autenticación básica, póngase en contacto con su administrador de cuentas.

1. Lea la advertencia y haga clic en **[!UICONTROL Confirmar credenciales]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si desea revisar las [asignaciones y personalizarlas](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), esta es su única oportunidad de hacerlo. Una vez que haga clic en [!UICONTROL Iniciar sincronización de Salesforce], habrá finalizado.

## Iniciar sincronización de [!DNL Salesforce] {#start-salesforce-sync}

1. Haga clic en **[!UICONTROL Iniciar sincronización de Salesforce]** para iniciar la sincronización persistente de Marketo-[!DNL Salesforce].

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de [!DNL Salesforce] ni cuando se introduzcan manualmente posibles clientes.

1. Haga clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >El tiempo para completar la sincronización inicial varía según el tamaño y la complejidad de la base de datos.

## Verificar sincronización {#verify-sync}

Marketo proporciona mensajes de estado para la sincronización de [!DNL Salesforce] en el área de administración. Puede comprobar que la sincronización funciona correctamente siguiendo estos pasos.

1. En Marketo, haz clic en **[!UICONTROL Admin]** y luego en **[!UICONTROL Salesforce]**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. El estado de sincronización es visible en la esquina superior derecha. Mostrará uno de los tres mensajes: **[!UICONTROL Última sincronización]**, **[!UICONTROL Sincronización en curso]** o **[!UICONTROL Error]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Acaba de terminar de configurar una de las funciones más potentes de Marketo. ¡Ya está!

>[!MORELIKETHIS]
>
>* [Paso 1 de 3: Agregar campos de Marketo a [!DNL Salesforce] (Empresa/ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Paso 2 de 3: Crear un [!DNL Salesforce] usuario para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Instalar el paquete Marketo Sales Insight en [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar Marketo Sales Insight en [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
