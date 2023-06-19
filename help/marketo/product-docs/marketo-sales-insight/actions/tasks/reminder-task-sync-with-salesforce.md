---
description: Sincronización de tareas de recordatorio con Salesforce - Documentos de Marketo - Documentación del producto
title: Sincronización de tareas de recordatorio con Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 1%

---

# Sincronización de tareas de recordatorio con Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para obtener información acerca de cómo habilitar la desprotección de sincronización de tareas [Sincronizar tareas/recordatorios de acciones de Sales Insight con tareas de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Una vez habilitada la configuración de sincronización de tareas, los usuarios verán sus tareas de recordatorio sincronizadas bidireccionalmente con Salesforce. Esto significa que los usuarios pueden administrar las tareas desde las acciones de Salesforce o Sales Insight y confiar en que los sistemas permanecerán alineados.

## Sincronización de campos de tarea de recordatorio {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

A continuación se muestra una lista de los campos de tarea de recordatorio de las acciones de perspectiva de ventas y sus campos de Salesforce correspondientes que se admiten mediante la sincronización de tareas bidireccional.

<table>
 <tr>
  <th>Campo de tarea de acciones de perspectiva de ventas</th>
  <th>Campo de tarea de Salesforce</th>
  <th>Tarea de Salesforce</th>
 </tr>
 <tr>
  <td>Nombre de tarea</td>
  <td>Campo de asunto</td>
  <td>Campo de resumen corto diseñado para mostrar el título de la tarea.</td>
 </tr>
 <tr>
  <td>Estado</td>
  <td>Estado de tarea</td>
  <td><p>Muestra el estado de la tarea. Las tareas de Acciones de perspectiva de ventas tienen dos estados que se asignan a dos de los valores de la lista desplegable Estado de la tarea de Salesforce.</p>
  <p>Abrir en Acciones de perspectiva de ventas = No iniciado en Salesforce.</p>
  <p>Completar en acciones de información de ventas = Completado en Salesforce.</p>
  <p>Los demás valores de estado de Salesforce no se sincronizarán con las acciones de información de ventas.</p></td>
 </tr>
 <tr>
  <td>Prioridad</td>
  <td>Prioridad</td>
  <td><p>La prioridad de acciones de perspectiva de ventas puede ser Normal o Alta, que se asigna a los valores de prioridad Normal y Alta en Salesforce.</p>
  <p>El valor de prioridad baja de Salesforce no se sincronizará con las acciones de información de ventas.</p></td>
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

## Sincronización de tareas de acciones de Sales Insight con Salesforce por primera vez {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Cuando active por primera vez la sincronización entre las acciones de Sales Insight y las tareas de Salesforce, importaremos sus tareas de Salesforce. Lo haremos **no** Pase cualquier tarea actual que tenga en Acciones de perspectiva de ventas a Salesforce. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan desde las acciones de información de ventas a Salesforce son las tareas creadas *después* Puede sincronizar las acciones de información de ventas con SFDC.

Esto es lo que sucede cuando sincroniza las acciones de Sales Insight y las tareas de SFDC:

* Tan pronto como haga clic en guardar en las tareas que se sincronizan, comienzan a sincronizarse. Inicialmente, esto llevará algún tiempo.

* Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se extraerá de SFDC a las acciones de información de ventas. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el Centro de comandos, solo verá las tareas con vencimiento hoy y mañana.

* Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, cualquier elemento que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

* Sincronizaremos constantemente las tareas entre las acciones de información de ventas y SFDC siempre y cuando la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en Acciones de Sales Insight se sincronizará con la lista de tareas en Salesforce. Y todo lo que se cree, edite, complete o elimine en Salesforce actualizará su lista de tareas en Acciones de perspectiva de ventas.

Para activar esta sincronización, simplemente marque la casilla de sincronización en su [Página Configuración](https://toutapp.com/login) en la aplicación web.

>[!NOTE]
>
>El campo de asunto de una tarea se puede actualizar en Sales Insight Actions y esa actualización se sincroniza en el campo de asunto de Salesforce para la tarea sincronizada correspondiente, si utiliza el campo `{{activity_subject}}` campo dinámico en su [Personalización de detalles de actividad](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) configuración. Por el contrario, cualquier actualización realizada en el campo de asunto en Salesforce _no_ Vaya al campo de asunto de la tarea Recordatorio de acciones de perspectiva de ventas.
