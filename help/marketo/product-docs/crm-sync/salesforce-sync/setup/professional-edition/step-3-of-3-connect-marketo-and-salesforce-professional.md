---
unique-page-id: 3571800
description: 'Paso 3 de 3: Conexión de Marketo y Salesforce (profesional): Documentos de Marketo: documentación del producto'
title: 'Paso 3 de 3: Conexión de Marketo y Salesforce (profesional)'
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo y [!DNL Salesforce] (Profesional) {#step-of-connect-marketo-and-salesforce-professional}

En este artículo, configurará Marketo Engage para que se sincronice con la instancia de Salesforce configurada.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: agregar campos de Marketo a Salesforce (profesional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [Paso 2 de 3: Crear un usuario de Salesforce para Marketo (profesional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## Recuperar token de seguridad de usuario de sincronización {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si ya tiene el token de seguridad, vaya directamente a Establecer credenciales de usuario de sincronización y felicitaciones para la preparación.

1. Inicie sesión en Salesforce con el usuario de sincronización de Marketo, haga clic en el nombre del usuario de sincronización y, a continuación, **[!UICONTROL Mi configuración]**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. En la barra de búsqueda de navegación, escriba &quot;restablecer&quot; y haga clic en **[!UICONTROL Restablecer mi token de seguridad]**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Haga clic en **[!UICONTROL Restablecer token de seguridad]**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   El token de seguridad se le enviará por correo electrónico.

## Establecer credenciales de usuario de sincronización {#set-sync-user-credentials}

1. En Marketo, ve a **[!UICONTROL Admin]**, selecciona **[!UICONTROL CRM]** y haz clic en **[!UICONTROL Sincronizar con Salesforce.com]**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Asegúrese de [ocultar todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} en Marketo del usuario de sincronización antes de hacer clic en **[!UICONTROL Campos de sincronización]**. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Escriba las credenciales del usuario de sincronización de Salesforce creadas en la parte 2 de la configuración de Salesforce ([Profesional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Empresa](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) y haga clic en **[!UICONTROL Campos de sincronización]**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marque **[!UICONTROL Sandbox]** si está sincronizando una zona protegida de Marketo con una de Salesforce.

1. Lea la advertencia y haga clic en **[!UICONTROL Confirmar credenciales]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si desea revisar las [asignaciones y personalizarlas](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}, esta es su única oportunidad de hacerlo. Una vez que haga clic en Iniciar sincronización de Salesforce, habrá finalizado.

## Iniciar sincronización de [!DNL Salesforce] {#start-salesforce-sync}

1. Haga clic en **[!UICONTROL Iniciar sincronización de Salesforce]** para iniciar la sincronización persistente entre Marketo y Salesforce.

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

1. En Marketo, haz clic en **[!UICONTROL Admin]** y luego en **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. El estado de sincronización es visible en la esquina superior derecha. Mostrará uno de los tres mensajes: **[!UICONTROL Última sincronización]**, **[!UICONTROL Sincronización en curso]** o **[!UICONTROL Error]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Acaba de terminar de configurar una de las funciones más potentes de Marketo. ¡Ya está!

>[!MORELIKETHIS]
>
>* [Instalar el paquete Marketo Sales Insight en Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configurar Marketo Sales Insight en Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}
