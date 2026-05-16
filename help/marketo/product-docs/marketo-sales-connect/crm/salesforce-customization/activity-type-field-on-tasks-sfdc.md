---
unique-page-id: 14352476
description: Comprenda el campo de tipo de actividad en las tareas al sincronizar Sales Connect con Salesforce. Consulte cómo se asignan y muestran los tipos de tareas en Salesforce.
title: Campo Tipo de actividad en tareas (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/UJAL2pE3Pq0n7Sn9ev7GMGkBbgx12pZ0I5lBzfLpF1c
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 5%

---

# Campo Tipo de actividad en tareas (SFDC) {#activity-type-field-on-tasks-sfdc}

Con la ayuda de [!DNL Sales Connect], puede registrar sus correos electrónicos y llamadas como una actividad en [!DNL Salesforce]. Una parte clave para tener datos valiosos en [!DNL Salesforce] es hacer que el campo [!UICONTROL Type] rellene el valor correcto.

>[!NOTE]
>
>Al registrar correos electrónicos a través de CCO no se verá la lista de selección de tipo de tarea, sino que se rellenará automáticamente el campo de tipo como &quot;correo electrónico&quot;, ya que se están enviando a [!DNL Salesforce] a través de su dirección de CCO.

## Requisitos {#requirements}

* Conexión con [!DNL Salesforce]
* No se ha seleccionado ningún valor de Tipo predeterminado en la lista desplegable Tipo de tarea
* Las opciones Llamar, Responder y Correo electrónico deben encontrarse en la lista de selección Tipo de tarea (el uso de mayúsculas es importante)
* Sin flujos de trabajo ni Déclencheur que realicen acciones en el valor del campo Tipo

## Configuración {#setup}

En primer lugar, compruebe que dispone de los valores correctos de la lista de selección. Necesitará la ayuda de su administrador de [!DNL Salesforce] para realizar cambios en la lista de selección.

1. Vaya a [Salesforce.com](https://salesforce.com) y haga clic en Configuración en la esquina superior derecha.
1. Haga clic en **[!UICONTROL Personalizar]**.
1. Haga clic en **[!UICONTROL Actividades]**.
1. Haga clic en **[!UICONTROL Campos de tarea]**.
1. Haga clic en **[!UICONTROL Tipo]**.
1. Ahora se encuentra en la Lista de selección de tipo de tarea. Asegúrese de que no haya seleccionado &quot;Predeterminado&quot;.
1. Asegúrese de que haya un valor [!UICONTROL Type] enumerado para [!UICONTROL Email], [!UICONTROL Call] y [!UICONTROL Reply].

Ahora que esto ya está hecho, empezará a ver que el campo Tipo rellena el valor correspondiente para los correos electrónicos, las llamadas y las respuestas registrados. Estos valores _no_ se rellenarán en las tareas de recordatorio de Sales Connect.

>[!NOTE]
>
>Si no ve &quot;Responder&quot; como valor, agréguelo haciendo clic en **[!UICONTROL Nuevo]**. &#39;Responder&#39; no es un valor estándar en [!DNL Salesforce].
