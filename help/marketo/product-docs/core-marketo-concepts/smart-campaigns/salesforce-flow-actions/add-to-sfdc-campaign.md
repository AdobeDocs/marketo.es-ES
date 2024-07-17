---
unique-page-id: 1147034
description: Añadir a la campaña de SFDC - Documentos de Marketo - Documentación del producto
title: Agregar a Campaña de SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 5%

---

# Agregar a Campaña de SFDC {#add-to-sfdc-campaign}

Este paso de flujo se puede utilizar en campañas de Marketo Engage o como un paso de flujo único para agregar personas como posibles clientes en una campaña de Salesforce. Si el posible cliente aún no existe en Salesforce, se sincronizará automáticamente y se agregará a la campaña con el estado especificado.

>[!NOTE]
>
>Solo está disponible cuando se integra con Salesforce.

![](assets/add-to-sfdc-campaign-1.png)

## Uso {#usage}

1. Busque y seleccione la campaña de Salesforce a la que desee agregar sus posibles clientes.

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >Si no puede ver una campaña de Salesforce en la lista de campañas:
   >
   >  1. Asegúrese de que la sincronización de campaña [esté habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
   >  1. Confirme que su [usuario de sincronización de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} es un [usuario de mercadotecnia](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} en Salesforce.

   >[!TIP]
   >
   >Puede usar la campaña de Salesforce [Mis tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} para facilitar la clonación de programas.

1. Seleccione el estado de miembro de la campaña de Salesforce que desee asignar a los posibles clientes cuando se añadan.

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >Si una persona ya es un miembro principal de la campaña de Salesforce, se omitirá y su estado NO se actualizará. En su lugar, puede usar [cambiar su estado en una campaña de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.
