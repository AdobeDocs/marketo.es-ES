---
unique-page-id: 2953469
description: 'Sincronización de SFDC: sincronización de Campaign: Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: sincronización de Campaign'
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 5%

---

# Sincronización de SFDC: sincronización de Campaign {#sfdc-sync-campaign-sync}

Los programas de Marketo se pueden sincronizar con [!DNL Salesforce] campañas. A continuación se muestra una descripción general de cómo funciona esto.

## ¿Por qué debería sincronizar los programas de Marketo con [!DNL Salesforce] campañas? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilice las potentes funciones de un programa de Marketo.
* Mantener a los miembros y su estado sincronizados entre un programa de Marketo y una campaña de [!DNL Salesforce].
* Aproveche las características de los informes de Marketo y [!DNL Salesforce].

## ¿Cómo se sincronizan un programa de Marketo y una campaña de [!DNL Salesforce]? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

En Marketo, tiene la opción de crear una asignación uno a uno entre un programa y una campaña [!DNL Salesforce].

![](assets/image2015-7-8-9-3a43-3a8.png)

El **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** y el **[costo de período](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** en Marketo se sincronizan con [!DNL Salesforce] como **tipo de campaña** y **costo real**. Esta sincronización es **unidireccional**, de Marketo a [!DNL Salesforce].

Los **miembros del programa** de Marketo y sus **[estados de progresión](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** se mantienen sincronizados con los **[!DNL Salesforce]miembros de campaña** y **estados de miembros de campaña**. Se trata de una **sincronización bidireccional**, por lo que cualquier cambio realizado en Marketo o [!DNL Salesforce] se reflejará en ambos sistemas.

>[!NOTE]
>
>Si hay miembros en el programa de Marketo que no existen en [!DNL Salesforce], Marketo crea esas personas como posibles clientes en [!DNL Salesforce].

## ¿Cuáles son los déclencheur relacionados con las campañas? {#what-are-the-triggers-filters-related-to-campaigns}

Desencadenadores:

* Se agregó a Campaña de SFDC
* Se quitó de Campaña de SFDC
* El estado está cambiado en la campaña de SFDC

Filtros:

* Miembro de la campaña SFDC

## ¿Puedo añadir Marketo People a mi campaña de SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sí, usar la acción de flujo [Agregar a SFDC campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Si esta persona no existe en [!DNL Salesforce], Marketo la creará en [!DNL Salesforce] y, a continuación, la agregará a la campaña.

## ¿Puedo eliminar miembros de mi campaña de SFDC mediante Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sí, usar la acción de flujo [Quitar de SFDC Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## ¿Puedo cambiar el estado de miembro de la campaña con Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sí, usar la acción de flujo [Cambiar estado en SFDC Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## ¿Por qué no puedo ver ninguna de mis [!DNL Salesforce] campañas? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Estas son las cosas que puede comprobar:

1. Asegúrese de que la sincronización de campaña [esté habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Confirme que su [usuario de sincronización de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) es un [usuario de mercadotecnia](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) en [!DNL Salesforce].

>[!NOTE]
>
>Si la campaña [!DNL Salesforce] y el programa de Marketo asignado tienen estados de programa incompatibles, es posible que reciba un mensaje de error. Le recomendamos que [coincida con los estados del programa anteriores a la sincronización](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Sincronizar una campaña de SFDC con un programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Explicación de la pertenencia al programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Habilitar/Deshabilitar sincronización de campaña](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Convertir al usuario de sincronización de Marketo en un usuario de mercadotecnia](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
