---
description: Sincronización de tareas de recordatorio con Salesforce - Documentos de Marketo - Documentación del producto
title: Sincronización de tareas de recordatorio con Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# Sincronización de tareas de recordatorio con Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para obtener información acerca de cómo habilitar la desprotección de sincronización de tareas [Sincronizar tareas/recordatorios de Sales Connect con tareas de Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Una vez habilitada la configuración de sincronización de tareas, los usuarios verán sus tareas de recordatorio sincronizadas bidireccionalmente con Salesforce. Esto significa que los usuarios pueden administrar las tareas desde Salesforce o Sales Connect y sentirse seguros de que los sistemas permanecerán alineados.

## Sincronización de campos de tarea de recordatorio {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

A continuación se muestra una lista de los campos de tarea de recordatorio de Sales Connect y sus campos de Salesforce correspondientes que se admiten mediante la sincronización de tareas bidireccional.

<table>
 <tr>
  <th>Campo de tarea de conexión de ventas</th>
  <th>Campo de tarea de Salesforce</th>
  <th>Tarea de Salesforce</th>
 </tr>
 <tr>
  <td>Nombre de la tarea</td>
  <td>Campo de asunto</td>
  <td>Campo de resumen corto diseñado para mostrar el título de la tarea.</td>
 </tr>
 <tr>
  <td>Estado</td>
  <td>Estado de tarea</td>
  <td><p>Muestra el estado de la tarea. Las tareas de Conexión de ventas tienen dos estados que se asignan a dos de los valores de la lista desplegable Estado de la tarea de Salesforce.</p>
  <p>Abrir en Sales Connect = No iniciado en Salesforce.</p>
  <p>Completar en Sales Connect = Completado en Salesforce.</p>
  <p>Los demás valores de estado de Salesforce no se sincronizarán con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Prioridad</td>
  <td>Prioridad</td>
  <td><p>La prioridad de Conexión de ventas puede ser Normal o Alta, que se asigna a los valores de prioridad Normal y Alta en Salesforce.</p>
  <p>El valor de prioridad baja de Salesforce no se sincronizará con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Fecha de vencimiento</td>
  <td>Fecha de vencimiento</td>
  <td>La fecha en la que vence la tarea.</td>
 </tr>
 <tr>
  <td>Detalles</td>
  <td>Comentarios</td>
  <td>Muestra información más detallada sobre lo que se pretendía completar con la tarea de recordatorio.</td>
 </tr>
</table>

## Sincronización de tareas de conexión de ventas con Salesforce por primera vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Cuando active por primera vez la sincronización entre las tareas de Sales Connect y Salesforce, importaremos sus tareas de Salesforce. Lo haremos **no** Pase cualquier tarea actual que tenga en Sales Connect a Salesforce. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan con Sales Connect son las creadas *después* se sincroniza Sales Connect con SFDC.

Esto es lo que sucede cuando sincroniza las tareas de Sales Connect y SFDC:

* Tan pronto como haga clic en guardar en las tareas que se sincronizan, comienzan a sincronizarse. Inicialmente, esto llevará algún tiempo.

* Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se recuperará de SFDC a Sales Connect. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el Centro de comandos, solo verá las tareas con vencimiento hoy y mañana.

* Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, cualquier elemento que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

* Siempre que la sincronización esté habilitada, sincronizaremos constantemente las tareas entre Sales Connect y SFDC.

Tras la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en Sales Connect se sincronizará con la lista de tareas de Salesforce. Y todo lo que se cree, edite, complete o elimine en Salesforce actualizará su lista de tareas en Sales Connect.

Para activar esta sincronización, simplemente marque la casilla de sincronización en su [Página Configuración](https://toutapp.com/login) en la aplicación web.

>[!NOTE]
>
>El campo de asunto de una tarea se puede actualizar en Sales Connect y esa actualización se sincroniza en el campo de asunto de Salesforce para la tarea sincronizada correspondiente, si utiliza el `{{activity_subject}}` campo dinámico en su [Personalización de detalles de actividad](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) configuración. Por el contrario, cualquier actualización realizada en el campo de asunto en Salesforce _no_ Vaya al campo de asunto de la tarea Recordatorio de Conexión de ventas.
