---
description: 'Paso 3 de 3: Marketo Engage de Connect y Veeva CRM: Marketo Docs: Documentación del producto'
title: 'Paso 3 de 3: Conexión del Marketo Engage y Veeva CRM'
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo Engage y Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

En este artículo, configurará el Marketo Engage para que se sincronice con la instancia de Veeva CRM configurada. **Verá Salesforce en algunas de las ventanas emergentes** ya que Veeva CRM está construido en la plataforma de Salesforce.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Añadir campos de Marketo a Veva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;}
>* [Paso 2 de 3: Crear un usuario de Veva para Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target=&quot;_blank&quot;}


>[!IMPORTANT]
>
>Solo se puede conectar una instancia de Marketo a una instancia de Veeva CRM a la vez.

## Conectarse a Veeva CRM mediante OAuth {#connect-to-veeva-crm-using-oauth}

1. En Marketo, Haga Clic En **Administrador**. Select **CRM** y haga clic en **Sincronización con Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Asegúrese de [ocultar todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target=&quot;_blank&quot;} en Marketo desde el usuario de sincronización antes de hacer clic en Sincronizar campos. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Haga clic en **Iniciar sesión con Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marque Sandbox si está sincronizando un Simulador para pruebas de Marketo con un Simulador para pruebas de Veeva CRM.

1. Haga clic en **Confirmar credenciales**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Aparecerá una ventana emergente con la página de inicio de sesión de Salesforce. Introduzca sus credenciales de &quot;usuario de sincronización de Marketo&quot; y haga clic en **Iniciar sesión**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Introduzca el código de verificación recibido por correo electrónico (enviado por Salesforce) y haga clic en **Verificar**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Cuando la verificación se realice correctamente, la página de acceso mostrará la solicitud de acceso. Haga clic en **Permitir**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. En unos minutos, aparecerá una ventana emergente en Marketo Engae. Haga clic en **Confirmar credenciales**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Iniciar sincronización de veeva {#start-veeva-sync}

1. Haga clic en **Iniciar sincronización de veeva** para iniciar la sincronización persistente de Marketo-Veva CRM.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente con una sincronización de Veeva CRM o cuando introduzca leads manualmente.

1. Haga clic en **Iniciar sincronización**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>El tiempo para completar la sincronización inicial varía según el tamaño y la complejidad de la base de datos.

## Verificar sincronización {#verify-sync}

Marketo proporciona mensajes de estado para la sincronización de Veva CRM en el área de administración. Puede verificar que la sincronización funciona correctamente siguiendo estos pasos.

1. En Marketo, haga clic en **Administrador**, luego **Véeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. El estado de sincronización es visible en la esquina superior derecha. Muestra uno de los tres mensajes siguientes: Última sincronización, sincronización en curso o error.

>[!MORELIKETHIS]
>
>[Configurar objetos personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}
