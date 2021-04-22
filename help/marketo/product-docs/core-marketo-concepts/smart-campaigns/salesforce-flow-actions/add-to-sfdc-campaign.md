---
unique-page-id: 1147034
description: Añadir a SFDC Campaign - Marketo Docs - Documentación del producto
title: Añadir a la campaña SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Agregar a la campaña SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Solo disponible cuando se integra con Salesforce.

## Información general {#overview}

Este paso de flujo se puede utilizar en campañas de Marketo o como un solo paso de flujo para añadir personas como posibles clientes en una campaña de Salesforce. Si el posible cliente aún no existe en Salesforce, se sincronizará automáticamente y se agregará a la campaña con el estado especificado.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Uso {#usage}

1. Busque y seleccione la campaña de Salesforce a la que desee agregar los posibles clientes.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Si no puede ver una campaña de Salesforce en la lista de campañas:
   >
   >  1. Asegúrese de que la [sincronización de campañas esté habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Confirme que su [usuario de sincronización de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) es [usuario de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) en Salesforce.


   >[!TIP]
   >
   >Puede utilizar la campaña [My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) de Salesforce para facilitar la clonación del programa.

1. Seleccione el estado de miembro de la campaña de Salesforce que desea asignar a los posibles clientes cuando se agreguen.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Si una persona ya es miembro principal de la campaña de Salesforce, se omitirá y su estado NO se actualizará. Puede utilizar [cambiar su estado en una campaña SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) en su lugar.
