---
description: 'Paso 3 de 3: Marketo Engage de Connect y Veeva CRM: Documentos de Marketo: documentación del producto'
title: 'Paso 3 de 3: Conectar Marketo Engage y Veeva CRM'
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Paso 3 de 3: Conectar Marketo Engage y Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

En este artículo, configurará Marketo Engage para que se sincronice con la instancia de Veeva CRM que ha configurado. **Verá Salesforce en algunas de las ventanas emergentes** as Veeva CRM se basa en la plataforma Salesforce.

>[!PREREQUISITES]
>
>* [Paso 1 de 3: Agregar campos de Marketo a Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Paso 2 de 3: Crear un usuario de Veeva para Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Solo se puede conectar una instancia de Marketo a una instancia de Veeva CRM a la vez.

## Conectarse a Veeva CRM mediante OAuth {#connect-to-veeva-crm-using-oauth}

1. En Marketo, Haga Clic En **Administrador**. Seleccionar **CRM** y haga clic en **Sincronización con Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Asegúrese de [ocultar todos los campos que no necesite](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} en Marketo desde el usuario de sincronización antes de hacer clic en Sincronizar campos. Una vez que haga clic en Sincronizar campos, todos los campos que el usuario pueda ver se crearán en Marketo de forma permanente y no se podrán eliminar.

1. Clic **Iniciar sesión con Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marque Zona protegida si va a sincronizar una Zona protegida de Marketo con una de Veeva CRM.

1. Clic **Confirmar credenciales**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Se mostrará una ventana emergente con la página de inicio de sesión de Salesforce. Introduzca las credenciales de &quot;Usuario de sincronización de Marketo&quot; y haga clic en **Iniciar sesión**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Introduzca el código de verificación que recibió por correo electrónico (enviado por Salesforce) y haga clic en **Verificar**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Una vez verificada correctamente, aparecerá la página de acceso que solicita el acceso. Clic **Permitir**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. En unos minutos, aparecerá una ventana emergente en Marketo Engage. Clic **Confirmar credenciales**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Iniciar sincronización de Veeva {#start-veeva-sync}

1. Clic **Iniciar sincronización de Veeva** para comenzar la sincronización persistente entre Marketo y Veeva CRM.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo no desduplicará automáticamente una sincronización de Veeva CRM o cuando introduzca manualmente posibles clientes.

1. Clic **Iniciar sincronización**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>El tiempo para completar la sincronización inicial varía según el tamaño y la complejidad de la base de datos.

## Verificar sincronización {#verify-sync}

Marketo proporciona mensajes de estado para la sincronización de Veeva CRM en el área de Administración. Puede comprobar que la sincronización funciona correctamente siguiendo estos pasos.

1. En Marketo, haga clic en **Administrador**, entonces **Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. El estado de sincronización es visible en la esquina superior derecha. Mostrará uno de los tres mensajes: Última sincronización, Sincronización en curso o Error.

>[!MORELIKETHIS]
>
>[Configuración de objetos personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
