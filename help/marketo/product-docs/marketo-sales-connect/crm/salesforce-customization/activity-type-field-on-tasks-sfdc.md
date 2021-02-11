---
unique-page-id: 14352476
description: Campo de tipo de actividad en Tareas (SFDC) - Documentos de marketing - Documentación del producto
title: Campo de tipo de actividad en Tareas (SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Campo de tipo de actividad en Tareas (SFDC) {#activity-type-field-on-tasks-sfdc}

Con la ayuda de Sales Connect, puede registrar sus correos electrónicos y llamadas como una actividad en Salesforce. Una parte clave para tener datos valiosos en Salesforce es que el campo Tipo rellene el valor correcto.

>[!NOTE]
>
>El registro de correos electrónicos a través de BCC no buscará en la lista de selección Tipo de Tarea y, en su lugar, rellenará automáticamente el campo de tipo como &quot;correo electrónico&quot;, ya que se enviarán a Salesforce a través de su dirección BCC.

## Requisitos {#requirements}

* Conexión con Salesforce
* No se seleccionó ningún valor de tipo predeterminado en la lista de selección de tipo de Tarea
* La llamada, la respuesta y el correo electrónico deben existir en la lista de selección Tipo de Tarea (la capitalización importa)
* Ningún Flujos de trabajo o Déclencheur que tome medidas sobre el valor del campo Tipo

## Configuración {#setup}

Primero compruebe que dispone de los valores de lista de selección correctos. Necesitará la ayuda de su administrador de Salesforce para realizar cualquier cambio en su lista de selección.

1. Vaya a [Salesforce.com](https://salesforce.com) y haga clic en Ajustes en la esquina superior derecha.
1. Haga clic en Personalizar.
1. Haga clic en Actividades.
1. Haga clic en Campos de Tarea.
1. Haga clic en Tipo.
1. Ahora está en la lista de selección de tipos de Tarea. Asegúrese de que no haya seleccionado &#39;Predeterminado&#39;.
1. Asegúrese de que hay un valor de tipo enumerado para Correo electrónico, Llamada y Respuesta.

Ahora que esto está en su lugar, comenzará a ver que el campo Tipo rellena el valor correspondiente para los correos electrónicos, las llamadas y las respuestas registrados. Estos valores **no** se rellenarán en las tareas de recordatorio de Sales Connect.

>[!NOTE]
>
>Si no ve &#39;Responder&#39; como un valor, agréguelo haciendo clic en **Nuevo**. &#39;Responder&#39; no es un valor estándar en Salesforce.
