---
unique-page-id: 2953469
description: 'Sincronización de SFDC: sincronización de campañas, documentos de Marketo, documentación del producto'
title: 'Sincronización de SFDC: sincronización de campaña'
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 5%

---

# Sincronización de SFDC: sincronización de campaña {#sfdc-sync-campaign-sync}

Los programas de Marketo se pueden sincronizar con campañas de Salesforce. A continuación se muestra una descripción general de cómo funciona esto.

## ¿Por qué debería sincronizar los programas de Marketo con las campañas de Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilice las potentes funciones de un programa de Marketo.
* Mantenga a los miembros y su estado sincronizados entre un programa de Marketo y una campaña de Salesforce.
* Aproveche las funciones de informes de Marketo y Salesforce.

## ¿Cómo se sincronizan un programa de Marketo y una campaña de Salesforce? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

En Marketo, tiene la opción de crear una asignación uno a uno entre un programa y una campaña de Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

El **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** y **[coste del período](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** en Marketo, sincronizar con Salesforce como **tipo de campaña** y **coste real**. Esta sincronización es **unidireccional**, de Marketo a Salesforce.

Marketo **miembros del programa** y sus **[estados de progresión](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** se mantienen sincronizados con el **Miembros de campaña de Salesforce** y **estados de miembros de campaña**. Este es un **sincronización bidireccional**, por lo que cualquier cambio realizado en Marketo o Salesforce se reflejará en ambos sistemas.

>[!NOTE]
>
>Si hay miembros en el programa de Marketo que no existen en Salesforce, Marketo crea esas personas como posibles clientes en Salesforce.

## ¿Cuáles son los déclencheur relacionados con las campañas? {#what-are-the-triggers-filters-related-to-campaigns}

Activadores:

* Se agregó a Campaña de SFDC
* Se quitó de Campaña de SFDC
* El estado está cambiado en la campaña de SFDC

Filtros:

* Miembro de la campaña SFDC

## ¿Puedo añadir Marketo People a mi campaña de SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sí, usar el [Añadir a la acción de flujo de campaña de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Si esta persona no existe en Salesforce, Marketo la creará en Salesforce y luego la agregará a la campaña.

## ¿Puedo eliminar miembros de mi campaña de SFDC mediante Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sí, usar el [Eliminar de la acción de flujo de la campaña SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## ¿Puedo cambiar el estado de miembro de la campaña con Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sí, usar el [Cambiar estado en la acción de flujo de la campaña SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## ¿Por qué no puedo ver ninguna de mis campañas de Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Estas son las cosas que puede comprobar:

1. Asegúrese de que la [la sincronización de campañas está habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Confirme que su [Usuario de sincronización de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) es un [Usuario de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) en Salesforce.

>[!NOTE]
>
>Si la campaña de Salesforce y el programa de Marketo asignado tienen estados de programa incompatibles, puede recibir un mensaje de error. Le recomendamos que [coincidir con los estados del programa anteriores a la sincronización](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Sincronización de una campaña de SFDC con un programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Explicación de la pertenencia al programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Habilitar/deshabilitar la sincronización de Campaign](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Convertir al usuario de sincronización de Marketo en usuario de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)
