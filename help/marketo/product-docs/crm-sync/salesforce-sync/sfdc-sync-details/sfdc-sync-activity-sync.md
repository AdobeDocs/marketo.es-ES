---
unique-page-id: 2953473
description: Sincronización de SFDC - Sincronización de Actividad - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: sincronización de Actividad'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Sincronización SFDC: Sincronización de actividad {#sfdc-sync-activity-sync}

Marketing también se sincroniza a través de los datos de actividades de Salesforce. Aquí hay algunas preguntas y respuestas.

## ¿Qué tipos de datos de actividad se sincronizan con Marketing? {#what-types-of-activity-data-does-marketo-sync-over}

El marketing se sincroniza sobre Eventos y Tareas asociadas con un posible cliente o contacto.

## ¿Cómo se mantienen sincronizados los detalles de actividad entre los dos sistemas? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La sincronización es de una manera, desde Salesforce hasta Marketing. Pero puede crear una tarea en Salesforce mediante el paso [Crear flujo de Tarea](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) o [Personalizar la sincronización](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) de Actividades con Salesforce.

## ¿Puedo crear una tarea con Marketing? {#can-i-create-a-task-using-marketo}

Sí, puede utilizar la acción [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)Crear flujo de Tarea.

## ¿Cuáles son los activadores/filtros relacionados con la actividad? {#what-are-the-triggers-filters-related-to-activity}

Activadores

* Actividad registrada
* Actividad actualizada

Filtros

* Se registró la actividad/No se registró la Actividad
* Se actualizó la actividad/No se actualizó la Actividad

>[!TIP]
>
>¿No está seguro de esa frase de &quot;No Actividad&quot;? El término &quot;no&quot; hace referencia a un filtro de inactividad. Más información sobre ellos aquí: [Usar Filtros de inactividad en una Lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

