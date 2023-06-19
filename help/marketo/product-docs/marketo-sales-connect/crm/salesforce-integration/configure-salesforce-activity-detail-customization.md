---
description: 'Configuración de la personalización de detalles de actividad de Salesforce: documentos de Marketo, documentación del producto'
title: Configurar la personalización de detalles de actividad de Salesforce
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Configurar la personalización de detalles de actividad de Salesforce {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce y Marketo Sales Connect [debe estar conectado](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* Registro de actividad de correo electrónico mediante API [debe estar habilitado](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)

La personalización de los detalles de actividad permite a los administradores configurar la información que se registra en el campo Tarea de Salesforce - Asunto, cuando se sincroniza una actividad de Conexión de ventas/tarea de recordatorio con Salesforce.

>[!NOTE]
>
>* Las actualizaciones realizadas en el campo de asunto en Sales Connect de una tarea de recordatorio se reflejarán en el campo de asunto de la tarea de Salesforce correspondiente, si está utilizando `{{activity_subject}}` Campo dinámico en la personalización de detalles de actividad.
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
  <td>Actividad de correo electrónico</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Actividad de llamada</td>
 </tr>
</table>

La función se puede utilizar para desbloquear las siguientes ventajas:

* Al personalizar qué información está visible en el campo de asunto, los detalles de la actividad se pueden analizar fácilmente para buscar ventas en Salesforce.
* Los administradores pueden etiquetar el campo de asunto con un identificador único como &quot;Mkto_sales&quot; para que las actividades de Sales Connect se puedan identificar y diferenciar fácilmente de otras actividades de correo electrónico, actividades de llamada y tareas.
* Reduzca la necesidad de campos de actividad personalizados. Salesforce impone límites al número de campos de actividad personalizados, lo cual puede restringir qué datos están disponibles para utilizarse en los informes. Si utiliza campos dinámicos de actividad para agregar datos clave a la línea de asunto, puede reducir el número de campos de actividad personalizados que necesita crear en la instancia de Salesforce.
* El campo de asunto de las actividades y tareas seguirá un patrón coherente definido por el administrador de Sales Connect.

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
>**Permisos de administración necesarios.**

Al configurar los detalles de la actividad, tenga en cuenta qué datos serían más relevantes para las ventas al revisar el historial de tareas en Salesforce.

1. Haga clic en el icono del engranaje y seleccione **Configuración**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Clic **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Clic **Configuración de sincronización**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. En el editor de personalización de detalles de actividad, añada el texto libre que desee. El texto que agregue no es dinámico y permanecerá sin cambios para el campo de asunto de todas las tareas sincronizadas con Salesforce.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Aunque no es obligatorio, ajustar el texto agregado entre corchetes puede facilitar a algunas personas la discernición entre los datos cuando se rellenan en un campo de asunto en Salesforce. Ejemplo: `[Sales Connect] - {{Activity_type}}`

1. Añada cualquier campo dinámico adicional que desee haciendo clic en el **Agregar campo dinámico** botón.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Seleccione los campos dinámicos que desee.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Clic **Guardar**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce impone un límite de 255 caracteres. Si los detalles de la actividad superan ese límite, se truncará para garantizar que la información se almacene en el campo de asunto de Salesforce.

>[!MORELIKETHIS]
>
>* [Configuración de sincronización](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronización de tareas de recordatorio con Salesforce](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [Personalización de Sales Connect para CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)
