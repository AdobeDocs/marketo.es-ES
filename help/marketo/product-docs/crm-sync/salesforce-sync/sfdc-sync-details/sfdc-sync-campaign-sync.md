---
unique-page-id: 2953469
description: 'Sincronización de SFDC: sincronización de campañas, documentos de Marketo, documentación del producto'
title: 'Sincronización de SFDC: sincronización de campaña'
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 5%

---

# Sincronización de SFDC: sincronización de campaña {#sfdc-sync-campaign-sync}

Los programas de Marketo Engage se pueden sincronizar con Campañas de Salesforce. A continuación se muestra una descripción general de cómo funciona esto.

## ¿Por qué debería sincronizar los programas de Marketo con las campañas de Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilice las potentes funciones de un programa de Marketo.
* Mantenga a los miembros y su estado sincronizados entre un programa de Marketo y una campaña de Salesforce.
* Aproveche las funciones de informes de Marketo y Salesforce.

## ¿Cómo se sincronizan un programa de Marketo y una campaña de Salesforce? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

En Marketo, tiene la opción de crear una asignación uno a uno entre un programa y una campaña de Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

El **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}** y el **[coste del período](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md){target="_blank"}** en Marketo se sincronizan con Salesforce como **tipo de campaña** y **coste real**. Esta sincronización es **unidireccional**, de Marketo a Salesforce.

Los **miembros del programa** de Marketo y sus **[estados de progresión](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}** se mantienen sincronizados con los **miembros de la campaña de Salesforce** y **estados de miembros de la campaña**. Se trata de una **sincronización bidireccional**, por lo que cualquier cambio realizado en Marketo o Salesforce se reflejará en ambos sistemas.

>[!NOTE]
>
>Si hay miembros en el programa de Marketo que no existen en Salesforce, Marketo crea esas personas como posibles clientes en Salesforce.

## ¿Cuáles son los déclencheur relacionados con las campañas? {#what-are-the-triggers-filters-related-to-campaigns}

Desencadenadores:

* Se agregó a Campaña de SFDC
* Se quitó de Campaña de SFDC
* El estado está cambiado en la campaña de SFDC

Filtros:

* Miembro de la campaña SFDC

## ¿Puedo añadir Marketo People a mi campaña de SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sí, usar la [acción de flujo Añadir a la campaña de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md){target="_blank"}. Si esta persona no existe en Salesforce, Marketo la creará en Salesforce y luego la agregará a la campaña.

## ¿Puedo eliminar miembros de mi campaña de SFDC mediante Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sí, usar la acción de flujo [Eliminar de la campaña de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## ¿Puedo cambiar el estado de miembro de la campaña con Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sí, usar la acción de flujo [Cambiar estado en la campaña de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## ¿Por qué no puedo ver ninguna de mis campañas de Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Estas son las cosas que puede comprobar:

1. Asegúrese de que la sincronización de campaña [esté habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
1. Confirme que su [usuario de sincronización de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} es un [usuario de mercadotecnia](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} en Salesforce.

>[!NOTE]
>
>Si la campaña de Salesforce y el programa de Marketo asignado tienen estados de programa incompatibles, puede recibir un mensaje de error. Le recomendamos que [coincida con los estados del programa anteriores a la sincronización](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Sincronizar una campaña de SFDC con un programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Explicación de la pertenencia al programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Habilitar/Deshabilitar sincronización de campaña](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Convertir al usuario de sincronización de Marketo en un usuario de mercadotecnia](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
