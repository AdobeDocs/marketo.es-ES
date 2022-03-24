---
description: 'Configuración de sincronización de Salesforce: Documentos de Marketo: Documentación del producto'
title: Configuración de sincronización de Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Configuración de sincronización de Salesforce {#salesforce-sync-settings}

## Registro de actividad de correo electrónico en Salesforce mediante API {#logging-email-activity-to-salesforce-via-api}

Esta funcionalidad requiere que esté en la edición Enterprise/Unlimited de Salesforce o en la edición Professional si ha comprado Integration a través de la API de servicios web.

>[!PREREQUISITES]
>
>Las acciones de Salesforce y Sales Insight deben estar conectadas.

1. En Acciones de perspectiva de ventas, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/salesforce-sync-settings-1.png)

1. En Configuración de administración (o &quot;Mi cuenta&quot; si no es administrador), haga clic en **Salesforce**.

   ![](assets/salesforce-sync-settings-2.png)

1. Haga clic en el **Configuración de sincronización** pestaña .

   ![](assets/salesforce-sync-settings-3.png)

1. Haga clic en la flecha situada junto a Registrar actividad de correo electrónico en Salesforce.

   ![](assets/salesforce-sync-settings-4.png)

1. Haga clic en el **API de Salesforce** pestaña . En esta tarjeta puede configurar su preferencia de información de registro en Salesforce. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/salesforce-sync-settings-5.png)

## Registro de actividades de correo electrónico en Salesforce mediante correo electrónico a Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Una vez que active &quot;Email to Salesforce (BCC)&quot;, recibirá un CCO de sus correos electrónicos de ventas y los mensajes de correo electrónico se registrarán como actividades sobre oportunidades, posibles clientes y contactos.

>[!PREREQUISITES]
>
>Las acciones de Salesforce y Sales Insight deben estar conectadas.

**Para registrar sus correos electrónicos en Salesforce por correo electrónico (BCC)**

1. En Ventas de Marketo, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/salesforce-sync-settings-6.png)

1. En Configuración de administración (o &quot;Mi cuenta&quot; si no es administrador), haga clic en **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. Haga clic en el **Configuración de sincronización** pestaña .

   ![](assets/salesforce-sync-settings-8.png)

1. Haga clic en el **Correo electrónico a Salesforce (BCC)** y haga clic en **Activar**.

   ![](assets/salesforce-sync-settings-9.png)

Si, por alguna razón, su dirección de correo electrónico a Salesforce no se introduce, siga estos pasos para activar la función de CCO en su cuenta de Salesforce:

1. Inicie sesión en la instancia de Salesforce.
1. Busque su nombre de usuario en la esquina superior derecha y seleccione la barra desplegable.
1. Select **Mis ajustes**.
1. Select **Correo electrónico**.
1. Select **Mi correo electrónico a Salesforce**.
1. En esta página, verá un campo etiquetado como &quot;Dirección de correo electrónico a Salesforce&quot;. Si no hay nada rellenado junto a él, desplácese hacia abajo hasta &quot;Mis direcciones de correo electrónico aceptables&quot;.
1. Introduzca las direcciones de correo electrónico que desea que sean CCO.
1. Haga clic en **Guardar cambios**.

**No encuentro mi correo electrónico para Salesforce en mi configuración**

Si no ve Mi correo electrónico a Salesforce en Configuración, es posible que el administrador no lo haya habilitado. Esto puede ocurrir si su equipo es nuevo en Salesforce o si su equipo nunca ha utilizado la dirección de CCO que proporciona Salesforce.

>[!NOTE]
>
>Necesitará privilegios de administrador para configurarlo.

1. Haga clic en **Configuración**.
1. Haga clic en **Administración de correo electrónico**.
1. Haga clic en **Enviar correo electrónico a Salesforce**.
1. Haga clic en **Editar**.
1. Marque la casilla junto a &quot;Activo&quot;.
1. Haga clic en **Guardar**.

## Sincronizar acciones de perspectivas de ventas Tareas/recordatorios con tareas de Salesforce {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. En Acciones de perspectiva de ventas, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/salesforce-sync-settings-10.png)

1. En Configuración de administración (o &quot;Mi cuenta&quot; si no es administrador), haga clic en **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. Haga clic en el **Configuración de sincronización** pestaña .

   ![](assets/salesforce-sync-settings-12.png)

1. Haga clic en la flecha situada junto a Sincronizar tareas/recordatorios de ventas de Marketo con tareas de Salesforce.

   ![](assets/salesforce-sync-settings-13.png)

1. Elija la opción deseada (&quot;No sincronizar con las tareas de Salesforce&quot; está seleccionada de forma predeterminada).

   ![](assets/salesforce-sync-settings-14.png)

## Sincronización de las tareas de las acciones de perspectiva de ventas con Salesforce por primera vez {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Cuando activa por primera vez la sincronización entre las acciones de perspectiva de ventas y las tareas de Salesforce, importamos sus tareas de Salesforce. No transferiremos a Salesforce ninguna tarea actual que tenga en Acciones de perspectivas de ventas. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan desde las acciones de perspectiva de ventas a Salesforce son las tareas creadas después de sincronizar las acciones de perspectiva de ventas con SFDC.

Esto es lo que sucede cuando sincroniza las acciones de perspectivas de ventas y las tareas de SFDC:

Tan pronto como haga clic en guardar en la sincronización de tareas, empezarán a sincronizarse. Inicialmente, esto llevará algún tiempo.

Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se extraerá de SFDC a las acciones de perspectiva de ventas. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el centro de comandos solo verá las tareas que vencen hoy y mañana.

Si la sincronización se ha activado anteriormente y elimina cualquier tarea en SFDC, todo lo que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

Sincronizaremos tareas constantemente entre las acciones de perspectiva de ventas y SFDC siempre y cuando la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en las acciones de perspectiva de ventas se sincronizará con la lista de tareas de Salesforce. Y todo lo que se cree, edite, complete o elimine en Salesforce actualizará su lista de tareas en Acciones de Insight de Ventas.

Para activar esta sincronización, marque la casilla de sincronización en la página Configuración de la aplicación web.
