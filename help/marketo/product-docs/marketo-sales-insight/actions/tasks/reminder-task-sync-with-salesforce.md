---
description: 'Sincronización de tareas de recordatorio con Salesforce: documentos de Marketo, documentación del producto'
title: Sincronización de tareas de recordatorio con Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Sincronización de tareas de recordatorio con [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para obtener información sobre cómo habilitar la sincronización de tareas, revisa [Sincronizar tareas/recordatorios de acciones de Insight de ventas con tareas de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Una vez habilitada la configuración de sincronización de tareas, los usuarios verán sus tareas de recordatorio sincronizadas bidireccionalmente con [!DNL Salesforce]. Esto significa que los usuarios pueden administrar tareas desde [!DNL Salesforce] o [!DNL Sales Insight Actions] y sentirse seguros de que los sistemas permanecerán alineados.

## Sincronización de campos de tarea de recordatorio {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

A continuación se muestra una lista de los campos de tarea de recordatorio de [!DNL Sales Insight Actions] y sus correspondientes [!DNL Salesforce] campos que se admiten mediante la sincronización de tareas bidireccional.

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] Campo de tarea</th>
  <th>[!DNL Salesforce] Campo de tarea</th>
  <th>[!DNL Salesforce] Tarea</th>
 </tr>
 <tr>
  <td>[!UICONTROL Nombre de tarea]</td>
  <td>[!UICONTROL Campo de asunto]</td>
  <td>Campo de resumen corto diseñado para mostrar el título de la tarea.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Estado]</td>
  <td>[!UICONTROL Estado de la tarea]</td>
  <td><p>Muestra el estado de la tarea. [!DNL Sales Insight Actions] tareas tienen dos estados que se asignan a dos de los valores de la lista de selección de estado de la tarea [!DNL Salesforce].</p>
  <p>Abrir en [!DNL Sales Insight Actions] = No iniciado en [!DNL Salesforce].</p>
  <p>Completar en [!DNL Sales Insight Actions] = Completado en [!DNL Salesforce].</p>
  <p>Los otros valores de estado de [!DNL Salesforce] no se sincronizarán con [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Prioridad]</td>
  <td>[!UICONTROL Prioridad]</td>
  <td><p>[!DNL Sales Insight Actions] la prioridad puede ser Normal o Alta, que se asigna a los valores de prioridad Normal y Alta de [!DNL Salesforce].</p>
  <p>El valor de prioridad baja de [!DNL Salesforce] no se sincronizará con [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Fecha de vencimiento]</td>
  <td>[!UICONTROL Fecha de vencimiento]</td>
  <td>La fecha en la que vence la tarea.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Detalles]</td>
  <td>[!UICONTROL Comentarios]</td>
  <td>Muestra información más detallada sobre lo que se pretendía completar con la tarea de recordatorio.</td>
 </tr>
</table>

## Sincronizando [!DNL Sales Insight Actions] tareas con [!DNL Salesforce] por primera vez {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

La primera vez que active la sincronización entre [!DNL Sales Insight Actions] y [!DNL Salesforce] tareas, importaremos sus [!DNL Salesforce] tareas. **no** insertaremos ninguna tarea actual que tenga en [!DNL Sales Insight Actions] a [!DNL Salesforce]. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan de [!DNL Sales Insight Actions] a [!DNL Salesforce] son las tareas creadas *después de* que sincronice [!DNL Sales Insight Actions] con SFDC.

Esto es lo que sucede cuando sincroniza [!DNL Sales Insight Actions] y tareas de SFDC:

* Tan pronto como haga clic en guardar en las tareas que se sincronizan, comienzan a sincronizarse. Inicialmente, esto llevará algún tiempo.

* Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se recuperará de SFDC a [!DNL Sales Insight Actions]. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el Centro de comandos, solo verá las tareas con vencimiento hoy y mañana.

* Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, cualquier elemento que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

* Sincronizaremos constantemente las tareas entre [!DNL Sales Insight Actions] y SFDC siempre y cuando la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en [!DNL Sales Insight Actions] se sincronizará con su lista de tareas en [!DNL Salesforce]. Y todo lo que se cree, edite, complete o elimine en [!DNL Salesforce] actualizará su lista de tareas en [!DNL Sales Insight Actions].

Para activar esta sincronización, simplemente marca la casilla de sincronización en tu [página de configuración](https://toutapp.com/login) en la aplicación web.

>[!NOTE]
>
>El campo de asunto de una tarea se puede actualizar en [!DNL Sales Insight Actions] y esa actualización se sincronizará en el campo de asunto [!DNL Salesforce] para la tarea sincronizada correspondiente, si está utilizando el campo dinámico `{{activity_subject}}` en la configuración de [Personalización de detalles de actividad](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). A la inversa, cualquier actualización realizada en el campo de asunto de [!DNL Salesforce] _no_ se sincronizará con el campo de asunto de la tarea de recordatorio [!DNL Sales Insight Actions].
