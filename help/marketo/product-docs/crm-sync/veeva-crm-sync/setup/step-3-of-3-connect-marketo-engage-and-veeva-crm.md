---
description: 'Paso 3 de 3: Conexión de Marketo Engage y  [!DNL Veeva] CRM: Documentos de Marketo: documentación del producto'
title: 'Paso 3 de 3: Conectar Marketo Engage y  [!DNL Veeva] CRM'
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo Engage y [!DNL Veeva] CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

En este artículo, configurará Marketo Engage para que se sincronice con su instancia de CRM [!DNL Veeva] configurada. **Verá [!DNL Salesforce] en algunas de las ventanas emergentes**, ya que [!DNL Veeva] CRM se ha creado en la plataforma [!DNL Salesforce].

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Agregar campos de Marketo a [!DNL Veeva]](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Paso 2 de 3: Crear un [!DNL Veeva] usuario para Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Solo se puede conectar una instancia de Marketo a una instancia de CRM [!DNL Veeva] a la vez.

## Conectar con [!DNL Veeva] CRM mediante OAuth {#connect-to-veeva-crm-using-oauth}

1. En Marketo, Haga Clic En **[!UICONTROL Administrador]**. Seleccione **[!UICONTROL CRM]** y haga clic en **[!UICONTROL Sincronizar con Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Asegúrese de [ocultar todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} en Marketo del usuario de sincronización antes de hacer clic en Sincronizar campos. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Haga clic en **[!UICONTROL Iniciar sesión con Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marque [!UICONTROL espacio aislado] si está sincronizando un espacio aislado de Marketo con un espacio aislado de CRM [!DNL Veeva].

1. Haga clic en **[!UICONTROL Confirmar credenciales]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Se mostrará una ventana emergente con la página de inicio de sesión [!DNL Salesforce]. Escriba sus credenciales de &quot;Usuario de sincronización de Marketo&quot; y haga clic en **[!UICONTROL Iniciar sesión]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Escriba el código de verificación que recibió por correo electrónico (enviado por [!DNL Salesforce]) y haga clic en **[!UICONTROL Verificar]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Una vez verificada correctamente, aparecerá la página de acceso que solicita el acceso. Haga clic en **[!UICONTROL Permitir]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. En unos minutos, aparecerá una ventana emergente en Marketo Engage. Haga clic en **[!UICONTROL Confirmar credenciales]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Iniciar sincronización de [!DNL Veeva] {#start-veeva-sync}

1. Haga clic en **[!UICONTROL Iniciar sincronización de Veeva]** para iniciar la sincronización persistente de CRM [!DNL Marketo-Veeva].

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de CRM [!DNL Veeva] ni cuando se introduzcan manualmente posibles clientes.

1. Haga clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>El tiempo para completar la sincronización inicial varía según el tamaño y la complejidad de la base de datos.

## Verificar sincronización {#verify-sync}

Marketo proporciona mensajes de estado para la sincronización de CRM [!DNL Veeva] en el área de administración. Puede comprobar que la sincronización funciona correctamente siguiendo estos pasos.

1. En Marketo, haz clic en **[!UICONTROL Admin]** y luego en **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. El estado de sincronización es visible en la esquina superior derecha. Mostrará uno de los tres mensajes: Última sincronización, Sincronización en curso o Error.

>[!MORELIKETHIS]
>
>[Configurar objetos personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
