---
unique-page-id: 2953469
description: Sincronización de SFDC - Sincronización de Campaña - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: sincronización de Campaña'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---


# Sincronización SFDC: Sincronización de campaña {#sfdc-sync-campaign-sync}

Los Programas de marketing se pueden sincronizar con Campañas de Salesforce. A continuación se muestra una descripción general de cómo funciona.

## ¿Por qué debo sincronizar los programas de marketing con las campañas de Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilice las potentes funciones de un Programa de marketing.
* Mantenga sincronizados los miembros y su estado entre un programa de marketing y una Campaña de Salesforce.
* Puntee en las funciones de sistema de informes de Marketing y Salesforce.

## ¿Cómo se sincronizan un Programa de marketing y una campaña de Salesforce? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

En Marketing, tiene la opción de crear una asignación uno a uno entre un programa y una campaña de Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

El costo [del](../../../../product-docs/administration/tags/create-a-program-channel.md) canal **** [y del](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** período ** en Marketing para sincronizar con Salesforce como tipo **de** campaña y costo **** real. Esta sincronización es de **una manera**, desde el Marketing hasta el Salesforce.

Los miembros **del** programa de marketing y sus estados [de](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)progresión *** se mantienen sincronizados con los miembros **de la campaña de** Salesforce y las estatuas **de los miembros de la** campaña. Se trata de una **sincronización** bidireccional ****, por lo que cualquier cambio realizado en Marketing o Salesforce se refleja en ambos sistemas.

>[!NOTE]
>
>Si hay miembros en el programa de mercadotecnia que no existen en Salesforce, Marketing crea a esas personas como leads en Salesforce.

## ¿Cuáles son los activadores/filtros relacionados con las campañas? {#what-are-the-triggers-filters-related-to-campaigns}

Desencadenadores:

* Añadido a la Campaña de SFDC
* Eliminado de la Campaña SFDC
* El estado se cambia en la Campaña de SFDC

Filtros:

* Miembro de la Campaña SFDC

## ¿Puedo agregar personas con marketing a mi campaña de SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sí, utilice la acción [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)Añadir a flujo de campaña SFDC. Si esta persona no existe en Salesforce, Marketing lo creará en Salesforce y luego lo agregará a la campaña.

## ¿Puedo eliminar miembros de mi campaña de SFDC mediante Marketing? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sí, utilice la acción [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)Eliminar del flujo de Campaña de SFDC.

## ¿Puedo cambiar el estado de los miembros de la campaña mediante el uso de Marketing? {#can-i-change-campaign-member-status-using-marketo}

Sí, utilice la acción [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)Cambiar estado en el flujo de Campaña SFDC.

## ¿Por qué no puedo ver ninguna de mis campañas de Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

A continuación se muestran algunas cosas que puede comprobar:

1. Asegúrese de que la sincronización de [campañas está activada](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Confirme que el usuario [de sincronización de](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) Marketing to es un usuario [de](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) marketing en Salesforce.

>[!NOTE]
>
>Si la campaña de Salesforce y el programa de marketing asignado tienen estados de programa incompatibles, puede recibir un mensaje de error. Se recomienda que [coincida con los estados de programa antes de la sincronización](sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Sincronizar una Campaña SFDC con un Programa](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Explicación de la pertenencia a Programa](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Activar/Desactivar sincronización de Campaña](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Hacer que el usuario de mercadotecnia sincronice con el usuario](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

>



