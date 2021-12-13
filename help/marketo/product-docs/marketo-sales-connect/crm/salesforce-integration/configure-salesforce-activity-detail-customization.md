---
description: 'Configurar la personalización de detalles de actividad de Salesforce: documentos de Marketo: documentación del producto'
title: Configurar la personalización de detalles de actividad de Salesforce
hide: true
hidefromtoc: true
source-git-commit: 137acd3ace0da73bcdfebcf7f4f2723bb03c7c39
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configurar la personalización de detalles de actividad de Salesforce {#configure-salesforce-activity-detail-customization}

La personalización de detalles de la actividad permite a los administradores configurar la información que se registrará en el campo Tarea de Salesforce - Asunto , cuando se sincronice una tarea de actividad/recordatorio de Conexión de ventas con Salesforce.

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Tarea de recordatorio de InMail</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>Actividad de correo electrónico</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Actividad de llamada</td>
 </tr>
</table>

La función se puede utilizar para obtener las siguientes ventajas:

* Al personalizar la información visible en el campo del asunto, los detalles de la actividad se pueden analizar fácilmente para ventas en Salesforce.
* Los administradores pueden etiquetar el campo del asunto con un identificador único como &quot;Mkto_sales&quot;, de modo que las actividades de Sales Connect se puedan identificar y diferenciar fácilmente de otras actividades de correo electrónico, actividades de llamada y tareas.
* Reduzca la necesidad de campos de actividad personalizados. Salesforce impone límites al número de campos de actividad personalizados, lo que puede restringir qué datos están disponibles para utilizarse en los informes. Al utilizar campos dinámicos de actividad para agregar datos clave a la línea de asunto, puede reducir el número de campos de actividad personalizados que necesita crear en la instancia de Salesforce.
* El campo de asunto de actividades y tareas seguirá un patrón coherente definido por el administrador de conexión de ventas.

## Campos dinámicos de actividad admitidos {#activity-dynamic-fields-supported}

Los campos dinámicos de actividad hacen referencia a información sobre las actividades de ventas para rellenar datos. Actualmente, se pueden utilizar con la personalización de detalles de actividad de Salesforce.

>[!NOTE]
>
>Si no hay ningún valor para rellenar el campo dinámico para una actividad/tarea específica, no rellenará ningún dato para ese campo dinámico cuando se actualice el campo Tarea - Asunto de Salesforce.

<table>
 <tr>
  <th>Campo</th>
  <th>Descripción</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Rellenará el tipo de tarea como Correo electrónico, Llamada, InMail o Personalizado.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Rellenará el asunto de la tarea.</p>
      <p>En el caso de un correo electrónico, se rellena la línea de asunto del correo electrónico.</p>
      <p>En el caso de llamada a , inMail o personalizado, rellenará un valor si hubo una tarea de recordatorio creada con un valor en el campo nombre/asunto de la tarea.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Si la actividad se inició desde una campaña de ventas, rellenará el nombre de la campaña de ventas.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Si la actividad se inició desde una campaña de ventas, rellenará el número de día de la campaña de ventas en el que se produjo esta actividad.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Si la actividad se inició desde una campaña de ventas, rellenará el número de paso dentro del día de la campaña de ventas en el que se produjo esta actividad.</td>
 </tr>
 <tr>
  <td>{{call_result}}</td>
  <td>Si la actividad es una llamada y se selecciona un resultado de llamada , se rellenará el valor del resultado de la llamada.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Si la actividad es una llamada y se selecciona un motivo de llamada, se rellenará el valor del motivo de la llamada.</td>
 </tr>
</table>

## Configuración de la personalización de detalles de actividad de Salesforce {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Se requieren permisos de administrador.**

Al configurar los detalles de la actividad, tenga en cuenta qué datos serían más relevantes para las ventas al revisar el historial de tareas en Salesforce.

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

PICC

1. Haga clic en **Salesforce**.

PICC

1. Haga clic en **Configuración de sincronización**.

PICC

1. En el editor Personalización de detalles de actividad añada cualquier texto libre que desee, este permanecerá sin cambios para el campo de asunto de todas las tareas sincronizadas con Salesforce.

1. Agregue los campos dinámicos que desee agregar haciendo clic en el botón de campo dinámico y seleccionando los campos dinámicos que desee utilizar en la lista.

1. Haga clic en **Guardar**.

>[!NOTE]
>
>Salesforce impone un límite de 255 caracteres. Si el detalle de la actividad supera ese límite, se truncará para garantizar que la información se pueda almacenar en el campo Asunto de Salesforce.

>[!MORELIKETHIS]
>
>* [Configuración de sincronización](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronización de tareas de recordatorio con Salesforce](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [Personalización de Sales Connect para CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)

