---
unique-page-id: 2953473
description: Sincronización SFDC - Sincronización de actividades - Documentos de Marketo - Documentación del producto
title: 'Sincronización de SFDC: Sincronización de actividades'
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 4%

---

# Sincronización SFDC: Sincronización de actividades {#sfdc-sync-activity-sync}

Marketo también se sincroniza sobre los datos de actividades de Salesforce. Aquí hay algunas preguntas y respuestas.

## ¿Qué tipos de datos de actividad sincroniza Marketo? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo se sincroniza tanto con Eventos como con Tareas asociadas a un posible cliente o contacto.

## ¿Cómo se sincronizan los detalles de la actividad entre los dos sistemas? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La sincronización es unidireccional, desde Salesforce a Marketo. Pero puede crear una tarea en Salesforce utilizando la variable [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) paso de flujo o [Personalizar sincronización de actividades](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) a Salesforce.

## ¿Puedo crear una tarea con Marketo? {#can-i-create-a-task-using-marketo}

Sí, puede usar la variable [Crear acción de flujo de tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## ¿Cuáles son los déclencheur o filtros relacionados con la actividad? {#what-are-the-triggers-filters-related-to-activity}

Desencadenadores

* La actividad está registrada
* La actividad está actualizada

Filtros

* Actividad registrada/No se registró actividad
* Actividad actualizada/Actividad no actualizada

>[!TIP]
>
>¿No está seguro de la redacción &quot;No es actividad&quot;? El término &quot;no&quot; hace referencia a un filtro de inactividad. Obtenga más información sobre ellos aquí: [Usar filtros de inactividad en una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
