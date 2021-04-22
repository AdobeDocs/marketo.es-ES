---
unique-page-id: 9437903
description: Crear un filtro de sincronización de Dynamics personalizado - Documentos de Marketo - Documentación del producto
title: Crear un filtro de sincronización de Dynamics personalizado
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Crear un filtro de sincronización de Dynamics personalizado {#create-a-custom-dynamics-sync-filter}

¿No desea sincronizar todo en su Dynamics CRM con Marketo? ¡No te preocupes! Marketo le permite configurar un filtro de sincronización y sincronizar solo parte de sus registros.

## Información general {#overview}

Para configurar un filtro de sincronización de Dynamics:

1. Cree un campo personalizado de dos opciones (booleano) denominado new_synctomkto en su Dynamics CRM para cualquier objeto (posible cliente, contacto, cuenta, oportunidad y otras entidades personalizadas).
1. Asigne este campo a un valor Sí/No o déjelo en blanco.

>[!NOTE]
>
>Debe realizar estos cambios en Dynamics CRM, no en la base de datos o en Marketo.

Marketo busca este campo durante la sincronización automática de fondo y determina qué registros se sincronizarán en función de esta lógica:

| Valor de campo | ¿Sincronizar con Marketo? |
|---|---|
| El campo no existe | Sí |
| El campo está vacío | Sí |
| El campo tiene valor Sí | Sí |
| El campo tiene valor No | No |

>[!CAUTION]
>
>La única manera de indicar a Marketo que omita un registro es establecer el valor del campo explícitamente como **No**. Marketo sigue sincronizando los registros aunque los valores de campo estén vacíos.

>[!PREREQUISITES]
>
>Instale la versión más reciente del complemento de Marketo (3.0.0.1 o posterior). Vaya a Marketo > Administración > Microsoft Dynamics > Descargar la solución de Marketo.

## Crear campo SyncToMkto {#create-synctomkto-field}

1. Inicie sesión en Dynamics CRM. Haga clic en **Configuración** y, a continuación, haga clic en **Personalizaciones**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Haga clic en **Personalizar el sistema**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Haga clic en ![](assets/image2015-8-10-21-3a44-3a23.png) junto a **Entities**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Haga clic en ![](assets/image2015-8-10-21-3a44-3a23.png) junto a **Lead** y seleccione **Fields**. A continuación, haga clic en **New**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Introduzca **SyncToMkto** en el campo **Display Name** y seleccione **Dos opciones** como **Data Type**. A continuación, haga clic en **Guardar y cerrar**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Elija cualquier nombre para mostrar para este campo, pero el campo Nombre debe ser exactamente **new_synctomkto**. Debe utilizar **new** como prefijo predeterminado. Si ha cambiado el valor predeterminado, vaya aquí a [restablecer el prefijo predeterminado para los nombres de campo personalizados](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md). Puede volver a cambiarlo después de crear los campos nuevos.

   >[!NOTE]
   >
   >Si tiene configurado un flujo de trabajo asincrónico, el registro obtiene el valor predeterminado SyncToMkto que ha configurado en el campo y obtiene el valor correcto unos segundos después, cuando el flujo de trabajo termina de ejecutarse. Si el valor predeterminado es Sí, esos registros se crearán en Marketo y después pasarán a estar obsoletos. Utilice **No** como valor predeterminado para evitar esto.

1. Repita este proceso y cree el campo **SyncToMkto** para cualquier otra entidad en la que desee limitar la sincronización, como entidades de contacto, cuenta, oportunidad y personalizadas.

## Seleccione el filtro en Marketo {#select-the-filter-in-marketo}

Incluso si ya ha realizado la sincronización inicial, entre y seleccione los campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Bueno, ahora ha habilitado el filtro de sincronización para Marketo.

## Crear un flujo de trabajo de Dynamics para asignar automáticamente valores de filtro de sincronización {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Siempre puede asignar manualmente un valor a los campos SyncToMkto para sus registros. Pero, ¿por qué no aprovechar la potencia de un flujo de trabajo de Dynamics y asignar automáticamente un valor al campo SyncToMkto cuando se crea o actualiza un registro?

>[!NOTE]
>
>No puede hacerlo en el nivel de base de datos. Debe realizarse en CRM manualmente o utilizando un flujo de trabajo.
>
>Un flujo de trabajo de Dynamics solo funciona con registros nuevos creados a partir de ahora, no con datos históricos. Utilice una actualización por lotes para pasar sobre registros existentes.

1. Vaya a Dynamics CRM. Haga clic en **Settings** y luego haga clic en **Processes**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Haga clic en **Nuevo**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Introduzca un nombre para el flujo de trabajo y seleccione **Workflow** como categoría y **Lead** como entidad. A continuación, haga clic en **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Cree reglas para asignar un valor verdadero o falso al campo **SyncToMkto** en función de las preferencias de su organización. Haga clic en **Guardar y cerrar**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Defina una acción predeterminada después de hacer clic en **Agregar paso** para agregar una condición de comprobación. Esto establece los registros que no desea sincronizar en **No**. De lo contrario, se sincronizarán.

1. Seleccione el flujo de trabajo y haga clic en **Activate**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consulte [Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) para configurar reglas que sincronicen solo registros para personas con direcciones de correo electrónico.

## Detalles del filtro de sincronización {#sync-filter-details}

A continuación, se muestran algunos detalles de implementación que pensamos que debe conocer:

1. Iniciar una operación de sincronización

   Cuando el valor **SyncToMkto** cambia de **No** a **Yes**, Dynamics notifica a Marketo inmediatamente para que inicie la sincronización de este registro. Si el registro ya existe, Marketo lo actualiza. De lo contrario, Marketo crea el registro.

   >[!TIP]
   >
   >Se agrega una operación `Create [StartSync]` al registro de Marketo cuando esto sucede.

1. Detener una operación de sincronización

   Cuando un registro cambia su valor SyncToMkto de Sí a No, se notifica a Marketo que deje de sincronizar este registro. Sin embargo, el registro no se elimina, sino que deja de recibir actualizaciones y se queda obsoleto.

>[!MORELIKETHIS]
>
>* [Filtro de sincronización de Microsoft Dynamics: Calificar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Filtro de sincronización de Microsoft Dynamics: Combinar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

