---
unique-page-id: 14352476
description: Campo de tipo de actividad en tareas (SFDC) - Documentos de Marketo - Documentación del producto
title: Campo Tipo de actividad en tareas (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# Campo Tipo de actividad en tareas (SFDC) {#activity-type-field-on-tasks-sfdc}

Con la ayuda de Sales Connect, puede registrar sus correos electrónicos y llamadas como actividad en Salesforce. Una parte clave para tener datos valiosos en Salesforce es que el campo Tipo rellene el valor correcto.

>[!NOTE]
>
>El registro de correos electrónicos a través de CCO no se realizará en la lista de selección de Tipo de tarea y, en su lugar, rellenará automáticamente el campo de tipo como &quot;correo electrónico&quot;, ya que se entregarán a Salesforce a través de su dirección CCO.

## Requisitos {#requirements}

* Conexión con Salesforce
* No se ha seleccionado ningún valor de Tipo predeterminado en la lista de selección Tipo de tarea
* La llamada, la respuesta y el correo electrónico deben existir en la lista de selección Tipo de tarea (el uso de mayúsculas y minúsculas es importante)
* No hay flujos de trabajo ni Déclencheur que realicen acciones en el valor del campo Tipo

## Instalación {#setup}

Primero compruebe que dispone de los valores de la lista de selección correctos. Necesitará la ayuda de su administrador de Salesforce para realizar cualquier cambio en su lista de selección.

1. Vaya a [Salesforce.com](https://salesforce.com) y haga clic en Configuración en la esquina superior derecha.
1. Haga clic en Personalizar.
1. Haga clic en Actividades.
1. Haga clic en Campos de tarea.
1. Tipo de clic.
1. Ahora se encuentra en la lista de selección Tipo de tarea. Asegúrese de que no haya seleccionado &#39;Predeterminado&#39;.
1. Asegúrese de que haya un valor Type enumerado para Correo electrónico, Llamada y Respuesta.

Una vez que esto esté listo, empezará a ver que el campo Tipo rellena el valor correspondiente para correos electrónicos, llamadas y respuestas registrados. Estos valores **not** se rellenarán en las tareas de recordatorio de Conexión de ventas.

>[!NOTE]
>
>Si no ve &quot;Responder&quot; como un valor, agréguelo haciendo clic en **Nuevo**. &#39;Reply&#39; no es un valor estándar en Salesforce.
