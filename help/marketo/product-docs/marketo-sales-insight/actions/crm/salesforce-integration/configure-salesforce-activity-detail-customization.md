---
description: 'Configuración de la personalización de detalles de actividad de Salesforce: documentos de Marketo, documentación del producto'
title: Configurar la personalización de detalles de actividad de Salesforce
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 1%

---

# Configurar la personalización de detalles de actividad de Salesforce {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Las acciones de Salesforce y Sales Insight [deben estar conectadas](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* El registro de la actividad de correo electrónico mediante la API [debe estar habilitado](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)

La personalización de los detalles de actividad permite a los administradores configurar la información que se registra en el campo Tarea de Salesforce - Asunto, cuando se sincroniza una actividad de Acciones de perspectiva de ventas/tarea de recordatorio con Salesforce.

>[!NOTE]
>
>* Las actualizaciones realizadas en el campo Asunto en las acciones de perspectiva de ventas de una tarea de recordatorio se reflejarán en el campo Asunto de la tarea de Salesforce correspondiente, si está utilizando el campo dinámico `{{activity_subject}}` en la personalización de los detalles de actividad.
>* Los saltos de línea no son compatibles al registrar información en el campo de asunto de Salesforce. Los saltos de línea del editor de personalización de detalles de actividad se eliminarán cuando se actualice el asunto de una tarea de ventas.

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Tarea de recordatorio de correo</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>Actividad de email</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Actividad de llamada</td>
 </tr>
</table>

La función se puede utilizar para desbloquear las siguientes ventajas:

* Al personalizar qué información está visible en el campo de asunto, los detalles de la actividad se pueden analizar fácilmente para buscar ventas en Salesforce.
* Los administradores pueden etiquetar el campo de asunto con un identificador único como &quot;Mkto_sales&quot; para que las actividades de las acciones de Sales Insight se puedan identificar y diferenciar fácilmente de otras actividades de correo electrónico, actividades de llamada y tareas.
* Reduzca la necesidad de campos de actividad personalizados. Salesforce impone límites al número de campos de actividad personalizados, lo cual puede restringir qué datos están disponibles para utilizarse en los informes. Si utiliza campos dinámicos de actividad para agregar datos clave a la línea de asunto, puede reducir el número de campos de actividad personalizados que necesita crear en la instancia de Salesforce.
* El campo de asunto de las actividades y tareas seguirá un patrón coherente definido por el administrador de acciones de Sales Insight.

>[!NOTE]
>
>Si está registrando las respuestas de correo electrónico como actividades de Salesforce, no se usará la configuración de personalización de detalles de actividad de Salesforce. En su lugar, registrarán como &quot;Respuesta: Asunto del correo electrónico&quot;.

## Campos dinámicos de actividad admitidos {#activity-dynamic-fields-supported}

Actividad Los campos dinámicos hacen referencia a información sobre sus actividades de ventas para rellenar datos. Actualmente, se pueden utilizar con la Personalización de detalles de actividad de Salesforce.

>[!NOTE]
>
>Si no hay ningún valor para rellenar el campo dinámico para una actividad o tarea específica, no rellenará ningún dato para ese campo dinámico cuando se actualice el campo Tarea de Salesforce - Asunto.

<table>
 <tr>
  <th>Campo</th>
  <th>Descripción</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Rellenará el tipo de tarea como Correo electrónico, Llamada, InMail o Personalizada.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Rellenará el asunto de la tarea.</p>
      <p>En el caso de un correo electrónico, rellena la línea de asunto del mismo.</p>
      <p>En el caso de la llamada, inMail o personalizada, rellena un valor si ha habido una tarea de recordatorio creada con un valor en el campo de nombre/asunto de la tarea.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Si la actividad se inició a partir de una campaña de ventas, se rellenará el nombre de la campaña de ventas.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Si la actividad se inició a partir de una campaña de ventas, se rellenará el número de día de campaña de ventas en el que se produjo esta actividad.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Si la actividad se inició a partir de una campaña de ventas, se rellenará el número de paso dentro del día de la campaña de ventas en el que se produjo esta actividad.</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>Si la actividad es una llamada y se selecciona un resultado de llamada, se rellenará el valor del resultado de la llamada.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Si la actividad es una llamada y se selecciona un motivo de llamada, se rellenará el valor del motivo de la llamada.</td>
 </tr>
</table>

## Configurar la personalización de detalles de actividad de Salesforce {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>Se requieren **permisos de administración.**

Al configurar los detalles de la actividad, tenga en cuenta qué datos serían más relevantes para las ventas al revisar el historial de tareas en Salesforce.

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Haga clic en **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Haga clic en **Configuración de sincronización**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. En el editor de personalización de detalles de actividad, añada el texto libre que desee. El texto que agregue no es dinámico y permanecerá sin cambios para el campo de asunto de todas las tareas sincronizadas con Salesforce.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Aunque no es obligatorio, ajustar el texto agregado entre corchetes puede facilitar a algunas personas la discernición entre los datos cuando se rellenan en un campo de asunto en Salesforce. Ejemplo: `[Sales Insight Actions] - {{Activity_type}}`

1. Agregue cualquier campo dinámico adicional que desee haciendo clic en el botón **Agregar campo dinámico**.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Seleccione los campos dinámicos que desee.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Haga clic en **Guardar**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce impone un límite de 255 caracteres. Si los detalles de la actividad superan ese límite, se truncará para garantizar que la información se almacene en el campo de asunto de Salesforce.

>[!MORELIKETHIS]
>
>* [Sincronizar actividades de ventas con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Sincronización de tareas de recordatorio con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
