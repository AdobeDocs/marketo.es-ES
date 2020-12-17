---
unique-page-id: 1147034
description: Añadir a la Campaña de SFDC - Documentos de marketing - Documentación del producto
title: Añadir a la Campaña de SFDC
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Añadir a la Campaña de SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Sólo disponible cuando se integra con Salesforce.

## Información general {#overview}

Este paso de flujo se puede utilizar en campañas de marketing o como un solo paso de flujo para agregar personas como posibles clientes en una campaña de Salesforce. Si el posible cliente aún no existe en Salesforce, se sincronizará automáticamente y se agregará a la campaña con el estado especificado.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Uso {#usage}

1. Busque y seleccione la campaña de Salesforce a la que desea agregar los leads.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Si no puede ver una campaña de Salesforce en la lista de Campaña:
   >
   >    
   >    
   >    1. Asegúrese de que la sincronización de [campaña está habilitada](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >    1. Confirme que el [usuario de sincronización de marketing](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) es [usuario de marketing](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) en Salesforce.


   >[!TIP]
   >
   >Puede utilizar la campaña de Salesforce [Mis tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) para facilitar la clonación de programas.

1. Seleccione el estado de miembro de campaña de Salesforce que desea asignar a los leads cuando se agreguen.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Si una persona ya es miembro principal de la campaña de Salesforce, se omitirán y NO se actualizará su estado. Puede utilizar [cambiar su estado en una campaña SFDC](change-status-in-sfdc-campaign.md) en su lugar.

