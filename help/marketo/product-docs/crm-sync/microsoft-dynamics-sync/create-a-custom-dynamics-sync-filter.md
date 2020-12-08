---
unique-page-id: 9437903
description: Creación de un filtro personalizado de sincronización dinámica - Documentos de marketing - Documentación del producto
title: Crear un filtro personalizado de sincronización de dinámica
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---


# Crear un filtro personalizado de sincronización de dinámica {#create-a-custom-dynamics-sync-filter}

¿No desea sincronizar todo en Dynamics CRM con Marketing? ¡No te preocupes! Marketo le permite configurar un filtro de sincronización y sincronizar sólo parte de sus registros.

## Información general {#overview}

Para configurar un filtro de sincronización de Dynamics:

1. Cree un campo personalizado de dos opciones (booleano) denominado new_synctomkto en su Dynamics CRM para cualquier objeto (posible cliente, contacto, cuenta, oportunidad y otras entidades personalizadas).
1. Asigne este campo un valor Sí/No o déjelo en blanco.

>[!NOTE]
>
>Debe realizar estos cambios en Dynamics CRM, no en la base de datos o en Marketing.

Marketo busca este campo durante la sincronización automática en segundo plano y determina qué registros sincronizar según esta lógica:

| Valor de campo | ¿Sincronizar con Marketing? |
|---|---|
| El campo no existe | Sí |
| El campo está vacío | Sí |
| El campo tiene el valor Sí | Sí |
| El campo tiene el valor No | No |

>[!CAUTION]
>
>La única manera de indicar a Marketing que omita un registro es establecer explícitamente el valor del campo en **No**. Marketo sigue sincronizando registros aunque los valores de campo estén vacíos.

>[!NOTE]
>
>**Requisitos previos**
>
>Instale la versión más reciente del complemento de marketing (3.0.0.1 o posterior). Vaya a Marketing > Administración > Microsoft Dynamics > Descargar solución de marketing.

## Crear campo SyncToMkto {#create-synctomkto-field}

1. Inicie sesión en Dynamics CRM. Haga clic en **Configuración** y, a continuación, en **Personalizaciones**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Haga clic en **Personalizar el sistema**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Haga clic en ![](assets/image2015-8-10-21-3a44-3a23.png) junto a **Entidades**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Haga clic ![](assets/image2015-8-10-21-3a44-3a23.png) junto a **Posible cliente **y seleccione **Campos**. A continuación, haga clic en **Nuevo**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Introduzca **SyncToMkto** en el campo **Nombre** para mostrar y seleccione **Dos opciones** como Tipo **de** datos. A continuación, haga clic en **Guardar y cerrar**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Elija cualquier nombre para mostrar para este campo, pero el campo Nombre debe ser exactamente **new_synctomkto**. Debe utilizar **new** como prefijo predeterminado. Si ha cambiado el valor predeterminado, vaya aquí para [restablecer el prefijo predeterminado para los nombres](create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md)de campo personalizados. Puede volver a cambiarlo después de crear los nuevos campos.

   >[!NOTE]
   >
   >Si tiene configurado un flujo de trabajo asincrónico, el registro obtiene el valor predeterminado SyncToMkto que configuró en el campo y obtiene el valor correcto unos segundos más tarde cuando el flujo de trabajo termina de ejecutarse. Si el valor predeterminado se establece en Sí, esos registros se crearán en el Explorador de mercadotecnia y, a continuación, pasarán a ser antiguos. Use **No** como valor predeterminado para evitarlo.

1. Repita este proceso y cree el campo **SyncToMkto** para cualquier otra entidad en la que desee limitar la sincronización, como entidades de contacto, cuenta, oportunidad y personalizadas.

## Seleccionar el filtro en el marketing {#select-the-filter-in-marketo}

Aunque ya haya realizado la sincronización inicial, vaya y seleccione los campos que se sincronizarán con Marketing.

1. Vaya a Administración y seleccione **MIcrosoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Haga clic en **Editar** en detalles de sincronización de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Desplácese hacia abajo hasta el campo y compruébelo. El nombre real debe ser new_synctomkto, pero el nombre para mostrar puede ser cualquier cosa. Haga clic en **Guardar**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Bueno, Ahora ha habilitado el filtro de sincronización para Marketing.

## Crear un flujo de trabajo de Dynamics para asignar automáticamente valores de filtro de sincronización {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Siempre puede asignar manualmente un valor a los campos SyncToMkto para sus registros. Pero, ¿por qué no aprovechar la potencia de un flujo de trabajo de Dynamics y asignar automáticamente un valor al campo SyncToMkto cuando se crea o actualiza un registro?

>[!NOTE]
>
>No puede hacerlo en el nivel de base de datos. Debe realizarse en la CRM manualmente o mediante un flujo de trabajo.
>
>Un flujo de trabajo de Dynamics solo funciona con registros nuevos creados a partir de ahora, no con datos históricos. Utilice una actualización por lotes para mover los registros existentes.

1. Vaya a Dynamics CRM. Haga clic en **Configuración** y luego en **Procesos**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Haga clic en **Nuevo**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Introduzca un nombre para el flujo de trabajo y seleccione **Flujo de trabajo** como categoría y **Posible cliente** como entidad. A continuación, haga clic en **Aceptar**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Cree reglas para asignar un valor verdadero o falso al campo **SyncToMkto** según las preferencias de su organización. Haga clic en **Guardar y cerrar**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Defina una acción predeterminada después de hacer clic en **Añadir paso** para agregar una condición de comprobación. Esto establece los registros que no desea sincronizar en **No**. De lo contrario, se sincronizarán.

1. Seleccione el flujo de trabajo y haga clic en **Activar**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consulte Reglas de filtro de sincronización [personalizada para obtener una dirección](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) de correo electrónico a fin de configurar las reglas para sincronizar solo los registros de las personas con direcciones de correo electrónico.

## Detalles del filtro de sincronización {#sync-filter-details}

A continuación, se muestran algunos detalles de implementación que pensamos que debe conocer:

1. Inicio de una operación de sincronización

   Cuando el valor **SyncToMkto** cambia de **No** a **Sí**, Dynamics notifica inmediatamente a Marketing al inicio que sincroniza este registro. Si el registro ya existe, Marketo lo actualiza. De lo contrario, Marketing crea el registro.

   >[!TIP]
   >
   >Cuando esto sucede, se agrega una operación **Create [StartSync]** al registro de marketing.

1. Detener una operación de sincronización

   Cuando un registro cambia su valor SyncToMkto de Sí a No, se notifica a Marketing que detendrá la sincronización de este registro. Sin embargo, el registro no se elimina, sino que deja de recibir actualizaciones y se queda anticuado.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Filtro de sincronización de Microsoft Dynamics: Calificar](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Filtro de sincronización de Microsoft Dynamics: Combinar](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

>



