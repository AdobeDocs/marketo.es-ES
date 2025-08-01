---
description: 'Sincronización de tareas de recordatorio con Salesforce: documentos de Marketo, documentación del producto'
title: Sincronización de tareas de recordatorio con Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Sincronización de tareas de recordatorio con [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para obtener información sobre cómo habilitar la sincronización de tareas, desproteja [Sincronizar [!DNL Sales Connect] Tareas/Recordatorios a [!DNL Salesforce] Tareas](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Una vez habilitada la configuración de sincronización de tareas, los usuarios verán sus tareas de recordatorio sincronizadas bidireccionalmente con [!DNL Salesforce]. Esto significa que los usuarios pueden administrar tareas desde [!DNL Salesforce] o [!DNL Sales Connect] y sentirse seguros de que los sistemas permanecerán alineados.

## Sincronización de campos de tarea de recordatorio {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

A continuación se muestra una lista de los campos de tarea de recordatorio de [!DNL Sales Connect] y sus correspondientes [!DNL Salesforce] campos que se admiten mediante la sincronización de tareas bidireccional.

<table>
 <tr>
  <th>[!DNL Sales Connect] Campo de tarea</th>
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
  <td><p>Muestra el estado de la tarea. [!DNL Sales Connect] tareas tienen dos estados que se asignan a dos de los valores de la lista de selección de estado de la tarea [!DNL Salesforce].</p>
  <p>Abrir en [!DNL Sales Connect] = No iniciado en [!DNL Salesforce].</p>
  <p>Completar en [!DNL Sales Connect] = Completado en [!DNL Salesforce].</p>
  <p>Los otros valores de estado de [!DNL Salesforce] no se sincronizarán con [!DNL Sales Connect].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Prioridad]</td>
  <td>[!UICONTROL Prioridad]</td>
  <td><p>[!DNL Sales Connect] la prioridad puede ser Normal o Alta, que se asigna a los valores de prioridad Normal y Alta de [!DNL Salesforce].</p>
  <p>El valor de prioridad baja de [!DNL Salesforce] no se sincronizará con [!DNL Sales Connect].</p></td>
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

## Sincronizando [!DNL Sales Connect] tareas con [!DNL Salesforce] por primera vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

La primera vez que active la sincronización entre [!DNL Sales Connect] y [!DNL Salesforce] tareas, importaremos sus [!DNL Salesforce] tareas. **no** insertaremos ninguna tarea actual que tenga en [!DNL Sales Connect] a [!DNL Salesforce]. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan de [!DNL Sales Connect] a [!DNL Salesforce] son las tareas creadas *después de* que sincronice [!DNL Sales Connect] con SFDC.

Esto es lo que sucede cuando sincroniza [!DNL Sales Connect] y tareas de SFDC:

* Tan pronto como haga clic en guardar en las tareas que se sincronizan, comienzan a sincronizarse. Inicialmente, esto llevará algún tiempo.

* Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se recuperará de SFDC a [!DNL Sales Connect]. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el Centro de comandos, solo verá las tareas con vencimiento hoy y mañana.

* Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, cualquier elemento que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

* Sincronizaremos constantemente las tareas entre [!DNL Sales Connect] y SFDC siempre y cuando la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en [!DNL Sales Connect] se sincronizará con su lista de tareas en [!DNL Salesforce]. Y todo lo que se cree, edite, complete o elimine en [!DNL Salesforce] actualizará su lista de tareas en [!DNL Sales Connect].

Para activar esta sincronización, simplemente marca la casilla de sincronización en tu [página de configuración](https://toutapp.com/login) en la aplicación web.

>[!NOTE]
>
>El campo de asunto de una tarea se puede actualizar en [!DNL Sales Connect] y esa actualización se sincronizará en el campo de asunto [!DNL Salesforce] para la tarea sincronizada correspondiente, si está utilizando el campo dinámico `{{activity_subject}}` en la configuración de [Personalización de detalles de actividad](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). A la inversa, cualquier actualización realizada en el campo de asunto de [!DNL Salesforce] _no_ se sincronizará con el campo de asunto de la tarea de recordatorio [!DNL Sales Connect].
