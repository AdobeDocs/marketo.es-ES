---
description: Sincronización de tareas de recordatorio con Salesforce - Marketo Docs - Documentación del producto
title: Sincronización de tareas de recordatorio con Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
source-git-commit: d2d6d4389f5a480afdfae6bfb62b9f48f0a2d88e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# Sincronización de tareas de recordatorio con Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para aprender a habilitar la sincronización de tareas, consulte [Sincronizar tareas/recordatorios de conexión de ventas con tareas de Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Una vez habilitada la configuración de sincronización de tareas, los usuarios verán sus tareas de recordatorio sincronizadas bidireccionalmente con Salesforce. Esto significa que los usuarios pueden administrar las tareas desde Salesforce o Sales Connect y confiar en que los sistemas permanecerán alineados.

## Sincronización de campos de tareas de recordatorio {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

A continuación, se muestra una lista de los campos de tareas recordatorias en Conexión de ventas y sus correspondientes campos de Salesforce que se admiten mediante la sincronización de tareas bidireccional.

<table>
 <tr>
  <th>Campo de tarea Conexión de Ventas</th>
  <th>Campo de tarea de Salesforce</th>
  <th>Tarea de Salesforce</th>
 </tr>
 <tr>
  <td>Nombre de la tarea</td>
  <td>Campo Asunto</td>
  <td>Campo de resumen breve que muestra el título de la tarea.</td>
 </tr>
 <tr>
  <td>Estado</td>
  <td>Estado de la tarea</td>
  <td><p>Muestra el estado de la tarea. Las tareas de conexión de ventas tienen dos estados que se asignan a dos de los valores de la lista de selección de estado de la tarea de Salesforce.</p>
  <p>Abrir en Conexión de ventas = No iniciado en Salesforce.</p>
  <p>Completar en Conexión de Ventas = Completado en Salesforce.</p>
  <p>Los demás valores de estado de Salesforce no se sincronizarán con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Prioridad</td>
  <td>Prioridad</td>
  <td><p>La prioridad Conexión de Ventas puede ser Normal o Alta, que se asigna a los valores de Prioridad Normal y Alta de Salesforce.</p>
  <p>El valor de baja prioridad de Salesforce no se sincronizará con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Fecha de vencimiento</td>
  <td>Fecha de vencimiento</td>
  <td>La fecha de vencimiento de la tarea.</td>
 </tr>
 <tr>
  <td>Detalles</td>
  <td>Comentarios</td>
  <td>Muestra información más detallada sobre lo que estaba pensado para completarse con la tarea de recordatorio.</td>
 </tr>
</table>

## Sincronización de tareas de conexión de ventas con Salesforce por primera vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Cuando activa por primera vez la sincronización entre las tareas de Conexión de ventas y Salesforce, importamos sus tareas de Salesforce. Nosotros **not** traspase cualquier tarea actual que tenga en Conexión de ventas a Salesforce. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan desde Conexión de ventas a Salesforce son las tareas creadas *after* sincroniza Sales Connect con SFDC.

Esto es lo que sucede cuando sincroniza las tareas de Conexión de ventas y SFDC:

* Tan pronto como haga clic en guardar en la sincronización de tareas, empezarán a sincronizarse. Inicialmente, esto llevará algún tiempo.

* Todos los recordatorios que se hayan actualizado o creado en las últimas 24 horas se extraerán de SFDC a Sales Connect. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el centro de comandos solo verá las tareas que vencen hoy y mañana.

* Si la sincronización se ha activado anteriormente y elimina cualquier tarea en SFDC, todo lo que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

* Sincronizaremos tareas constantemente entre Sales Connect y SFDC siempre que la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en Sales Connect se sincronizará con la lista de tareas de Salesforce. Y todo lo creado, editado, completado o eliminado en Salesforce actualizará su lista de tareas en Conexión de ventas.

Para activar esta sincronización, marque la casilla de sincronización en su [Página Configuración](https://toutapp.com/login) en la aplicación web.

>[!NOTE]
>
>El campo de asunto de una tarea se puede actualizar en Conexión de ventas y esa actualización se sincronizará en el campo de asunto de Salesforce para la tarea sincronizada correspondiente, si está utilizando la variable `{{activity_subject}}` el campo dinámico del [Personalización de los detalles de la actividad](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) configuración. Por el contrario, cualquier actualización realizada en el campo de asunto en Salesforce _not_ sincronice con el campo del asunto de la tarea recordatorio de conexión de ventas.
