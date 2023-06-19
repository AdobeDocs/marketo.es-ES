---
description: Actualizar el campo Tipo de actividad al registrar actividades en Salesforce - Documentos de Marketo - Documentación del producto
title: Actualizar el campo Tipo de actividad al registrar actividades en Salesforce
exl-id: f65d7d97-ec65-4210-9381-02be788498f9
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Actualizar el campo Tipo de actividad al registrar actividades en Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

Las acciones pueden sincronizar automáticamente el correo electrónico y las actividades de llamada con Salesforce para su uso en la creación de informes y aumentar la visibilidad en el historial de actividades. Al registrar actividades, asegúrese de que el campo Tipo de actividad se actualiza correctamente a Correo electrónico, Llamada o Respuesta, según el tipo de actividad que se esté registrando.

>[!NOTE]
>
>Al registrar correos electrónicos a través de CCO no se verá la lista de selección de tipo de tarea, sino que se rellenará automáticamente el campo de tipo como &quot;correo electrónico&quot;, ya que se envían a Salesforce a través de su dirección de CCO.

## Cosas que saber {#things-to-know}

* Se requiere una conexión con Salesforce para que el tipo de tarea se actualice.
* No debe haber ningún valor Tipo predeterminado seleccionado en la lista desplegable Tipo de tarea.
* Las opciones Llamar, Responder y Correo electrónico deben estar incluidas en la lista de selección Tipo de tarea (el uso de mayúsculas es importante).
* Los flujos de trabajo o Déclencheur de Salesforce que actualizan el campo Tipo de tarea pueden interferir con este proceso.

## Instalación {#setup}

En primer lugar, compruebe que dispone de los valores correctos de la lista de selección. Necesitará la ayuda de su administrador de Salesforce para realizar cambios en la lista de selección.

Primero compruebe qué valores le faltan en la lista de selección de tipo de tarea (sin correo electrónico, llamada y respuesta). Es posible que necesite la ayuda de su administrador de Salesforce para revisar esto y realizar cambios en la lista de selección del tipo de actividad. Para realizar estos cambios, su administrador de Salesforce puede seguir los pasos a continuación.

### En Salesforce Lightning {#salesforce-lightning}

1. Vaya a [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Haga clic en el icono de engranaje en la esquina superior derecha y seleccione **Configurar** > **Administrador de objetos**.
1. Escriba &quot;task&quot; en el cuadro &quot;Búsqueda rápida&quot;.
1. En el panel izquierdo, haga clic en **Campos y relaciones**.
1. Etiqueta de campo de clic **Tipo**.
1. En Valor de lista de selección de tipo de tarea, haga clic en **Nuevo**.
1. Escriba el nombre de los valores de la lista de selección de tipo de tarea que faltan (&quot;Correo electrónico, &quot;Llamada&quot;, &quot;Respuesta&quot;).
1. Clic **Guardar**.

### En Salesforce Classic {#salesforce-classic}

1. Vaya a [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Clic **Configurar** > **Generar** > **Personalizar** > **Actividades** > **Campos de tarea**.
1. Clic **Tipo**.
1. En Valor de lista de selección de tipo de tarea, haga clic en **Nuevo**.
1. Escriba el nombre de los valores de la lista de selección de tipo de tarea que faltan (&quot;Correo electrónico, &quot;Llamada&quot;, &quot;Respuesta&quot;).
1. Clic **Guardar**.

Ahora que esto ya está hecho, empezará a ver que el campo Tipo rellena el valor correspondiente para los correos electrónicos, las llamadas y las respuestas registrados. Estos valores: _no_ se rellenarán en las tareas de recordatorio de Acciones de perspectiva de ventas.

>[!NOTE]
>
>Si no ve &quot;Responder&quot; como valor, agréguelo haciendo clic en **Nuevo**. &#39;Responder&#39; no es un valor estándar en Salesforce.

>[!MORELIKETHIS]
>
>* [Registro de atributos de actividad de ventas en Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Configurar la personalización de detalles de actividad de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Sincronizar actividades de ventas con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
