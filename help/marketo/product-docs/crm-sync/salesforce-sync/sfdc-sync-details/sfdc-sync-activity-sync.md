---
unique-page-id: 2953473
description: Obtenga información acerca de cómo las actividades y tareas de Salesforce se sincronizan con Marketo. Cree tareas desde Marketo y utilice déclencheur y filtros de actividad en campañas inteligentes.
title: 'Sincronización de SFDC: sincronización de actividades'
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/N-pw1q0NXaJGKW1J1R4iqhgXhA42sX5nP0OWPXCuaBc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 6%

---

# Sincronización de SFDC: sincronización de actividades {#sfdc-sync-activity-sync}

Marketo también sincroniza los datos de las actividades [!DNL Salesforce]. Estas son algunas preguntas y respuestas.

## ¿Con qué tipos de datos de actividad se sincroniza Marketo? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo se sincroniza entre los eventos y las tareas asociados con un posible cliente o contacto.

## ¿Cómo se sincronizan los detalles de la actividad entre los dos sistemas? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La sincronización es unidireccional, de [!DNL Salesforce] a Marketo. Pero puede crear una tarea en [!DNL Salesforce] mediante el paso de flujo [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) o [Personalizar sincronización de actividades](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) a [!DNL Salesforce].

## ¿Puedo crear una tarea con Marketo? {#can-i-create-a-task-using-marketo}

Sí, puede usar la [acción Crear flujo de tareas](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## ¿Cuáles son los déclencheur relacionados con la actividad? {#what-are-the-triggers-filters-related-to-activity}

Activadores

* La actividad está registrada
* La actividad está actualizada

Filtros

* Se registró la actividad/no se registró la actividad
* La actividad se ha actualizado/No se ha actualizado la actividad

>[!TIP]
>
>¿No está seguro de la frase &quot;Sin actividad&quot;? La opción &quot;no&quot; hace referencia a un filtro de inactividad. Obtenga más información sobre ellos aquí: [Usar filtros de inactividad en una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
