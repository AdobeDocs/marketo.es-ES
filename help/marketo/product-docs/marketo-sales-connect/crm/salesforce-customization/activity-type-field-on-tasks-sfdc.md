---
unique-page-id: 14352476
description: Campo de tipo de actividad en tareas (SFDC) - Documentos de Marketo - Documentación del producto
title: Campo de tipo de actividad en tareas (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# Campo de tipo de actividad en tareas (SFDC) {#activity-type-field-on-tasks-sfdc}

Con la ayuda de Sales Connect puede registrar sus correos electrónicos y llamadas como una actividad en Salesforce. Una parte clave para tener datos valiosos en Salesforce es hacer que el campo Tipo rellene el valor correcto.

>[!NOTE]
>
>Al registrar correos electrónicos a través de CCO no se verá la lista de selección de tipo de tarea, sino que se rellenará automáticamente el campo de tipo como &quot;correo electrónico&quot;, ya que se entregan a Salesforce a través de su dirección de CCO.

## Requisitos {#requirements}

* Conexión con Salesforce
* No se ha seleccionado ningún valor de Tipo predeterminado en la lista desplegable Tipo de tarea
* Las opciones Llamar, Responder y Correo electrónico deben encontrarse en la lista de selección Tipo de tarea (el uso de mayúsculas es importante)
* Sin flujos de trabajo ni Déclencheur que realicen acciones en el valor del campo Tipo

## Instalación {#setup}

En primer lugar, compruebe que dispone de los valores correctos de la lista de selección. Necesitará la ayuda de su administrador de Salesforce para realizar cambios en la lista de selección.

1. Vaya a [Salesforce.com](https://salesforce.com) y haga clic en Configuración en la esquina superior derecha.
1. Haga clic en Personalizar.
1. Haga clic en Actividades.
1. Haga clic en Campos de tarea.
1. Tipo de clic.
1. Ahora se encuentra en la Lista de selección de tipo de tarea. Asegúrese de que no haya seleccionado &quot;Predeterminado&quot;.
1. Asegúrese de que haya un valor Tipo en la lista para Correo electrónico, Llamada y Respuesta.

Ahora que esto ya está hecho, empezará a ver que el campo Tipo rellena el valor correspondiente para los correos electrónicos, las llamadas y las respuestas registrados. Estos valores: _no_ se rellenarán en las tareas de recordatorio de Conexión de ventas.

>[!NOTE]
>
>Si no ve &quot;Responder&quot; como valor, agréguelo haciendo clic en **Nuevo**. &#39;Responder&#39; no es un valor estándar en Salesforce.
