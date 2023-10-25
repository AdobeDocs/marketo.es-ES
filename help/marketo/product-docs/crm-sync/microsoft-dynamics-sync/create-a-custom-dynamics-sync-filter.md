---
unique-page-id: 9437903
description: 'Creación de un filtro de sincronización de Dynamics personalizado: documentos de Marketo, documentación del producto'
title: Crear un filtro de sincronización personalizado de Dynamics
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Crear un filtro de sincronización personalizado de Dynamics {#create-a-custom-dynamics-sync-filter}

¿No desea sincronizar todo el contenido de su Dynamics CRM con Marketo? ¡No te preocupes! Marketo le permite configurar un filtro de sincronización y sincronizar solo parte de los registros.

## Información general {#overview}

Para configurar un filtro de sincronización de Dynamics:

1. Cree un campo personalizado de dos opciones (booleano) denominado new_synctomkto en Dynamics CRM para cualquier objeto (posible cliente, contacto, cuenta, oportunidad y otras entidades personalizadas).
1. Asigne un valor Sí/No a este campo o déjelo en blanco.

>[!NOTE]
>
>Debe realizar estos cambios en Dynamics CRM, no en la base de datos o en Marketo.

Marketo busca este campo durante la sincronización automática en segundo plano y determina qué registros se sincronizan según esta lógica:

| Valor de campo | ¿Sincronizar con Marketo? |
|---|---|
| El campo no existe | Sí |
| El campo está vacío | Sí |
| El campo tiene el valor Sí | Sí |
| El campo tiene el valor No | No |

>[!CAUTION]
>
>La única manera de indicar a Marketo que omita un registro es establecer el valor del campo explícitamente para que sea **No**. Marketo sigue sincronizando registros aunque los valores de los campos estén vacíos.

>[!PREREQUISITES]
>
>Instale la última versión del complemento de Marketo (3.0.0.1 o posterior). Vaya a Marketo > Administración > Microsoft Dynamics > Descargar solución de Marketo.

## Crear campo SyncToMkto {#create-synctomkto-field}

1. Inicie sesión en Dynamics CRM. Clic **Configuración**, luego haga clic en **Personalizaciones**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Clic **Personalizar el sistema**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Clic ![](assets/image2015-8-10-21-3a44-3a23.png) junto a **Entidades**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Clic ![](assets/image2015-8-10-21-3a44-3a23.png) junto a **Posible cliente** y seleccione **Campos**. Luego haga clic en **Nuevo**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Entrar **SyncToMkto** en el **Nombre para mostrar** y seleccione **Dos opciones** como el **Tipo de datos**. Luego haga clic en **Guardar y cerrar**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Elija cualquier nombre para mostrar para este campo, pero el campo Nombre debe ser exactamente **new_synctomkto**. Debe utilizar **nuevo** como prefijo predeterminado. Si ha cambiado el valor predeterminado, vaya aquí para [restablecer el prefijo predeterminado para los nombres de campo personalizados](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Puede volver a cambiarlo después de crear los nuevos campos.

   >[!NOTE]
   >
   >Si tiene configurado un flujo de trabajo asincrónico, el registro obtiene el valor predeterminado de SyncToMkto configurado en el campo y obtiene el valor correcto unos segundos más tarde, cuando el flujo de trabajo termina de ejecutarse. Si el valor predeterminado se establece en Yes, esos registros se crean en Marketo y quedan obsoletos. Uso **No** como valor predeterminado para evitarlo.

1. Repita este proceso y cree el **SyncToMkto** para cualquier otra entidad en la que desee limitar la sincronización, como entidades de contacto, cuenta, oportunidad y personalizadas.

## Seleccione el filtro en Marketo {#select-the-filter-in-marketo}

Incluso si ya ha realizado la sincronización inicial, entre y seleccione los campos que desea sincronizar con Marketo.

1. Vaya a Administración y seleccione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clic **[!UICONTROL Editar]** en Detalles de sincronización de campos.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el Nombre para mostrar puede ser cualquier cosa. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Genial. Ahora ha habilitado el filtro de sincronización para Marketo.

## Crear un flujo de trabajo de Dynamics para asignar valores de filtro de sincronización automáticamente {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Siempre puede asignar manualmente un valor a los campos SyncToMkto de los registros. Pero, ¿por qué no aprovechar la potencia de un flujo de trabajo de Dynamics y asignar automáticamente un valor al campo SyncToMkto cuando se crea o actualiza un registro?

>[!NOTE]
>
>No se puede hacer esto en la base de datos. Debe realizarse en CRM manualmente o mediante un flujo de trabajo.
>
>Un flujo de trabajo de Dynamics solo funciona en registros nuevos creados a partir de ahora, no en datos históricos. Utilice una actualización por lotes para pasar sobre los registros existentes.

1. Vaya a Dynamics CRM. Clic **Configuración**, entonces **Procesos**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Clic **Nuevo**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Introduzca un nombre para el flujo de trabajo y seleccione **Flujo de trabajo** como la categoría y **Posible cliente** como la entidad. Luego haga clic en **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Cree reglas para asignar un valor verdadero o falso al **SyncToMkto** en función de las preferencias de su organización. Clic **Guardar y cerrar**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Defina una Acción predeterminada después de hacer clic en **Añadir etapa** para añadir una condición de comprobación. Esto establece los registros con los que no se desea sincronizar **No**. De lo contrario, se sincronizarán.

1. Seleccione el flujo de trabajo y haga clic en **Activar**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consulte [Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} para configurar reglas para sincronizar solo registros para personas con direcciones de correo electrónico.

## Detalles del filtro de sincronización {#sync-filter-details}

Estos son algunos detalles de la implementación que pensamos que debería conocer:

* Iniciar una operación de sincronización

  Si la variable **SyncToMkto** el valor cambia de **No** hasta **Sí**, Dynamics notifica a Marketo inmediatamente para que inicie la sincronización de este registro. Si el registro ya existe, Marketo lo actualiza. De lo contrario, Marketo crea el registro.

  >[!TIP]
  >
  >A `Create [StartSync]` operación se añade al registro de Marketo cuando esto sucede.

* Detener una operación de sincronización

  Cuando un registro cambia su valor SyncToMkto de Sí a No, se notifica a Marketo que deje de sincronizar este registro. Sin embargo, el registro no se elimina; en su lugar, deja de recibir actualizaciones y se vuelve obsoleto.

>[!MORELIKETHIS]
>
>* [Filtro de sincronización de Microsoft Dynamics: Calificar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Filtro de sincronización de Microsoft Dynamics: Combinar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
