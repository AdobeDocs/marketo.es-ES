---
unique-page-id: 1147034
description: Añadir a la Campaña de SFDC - Documentos de marketing - Documentación del producto
title: Añadir a la Campaña de SFDC
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Añadir a la Campaña de SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

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
   >    1. Asegúrese de que la sincronización de [campañas está activada](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >    1. Confirme que el usuario [de sincronización de](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) Marketing to es un usuario [de](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) marketing en Salesforce.


   >[!TIP]
   >
   >Puede utilizar la campaña de Salesforce [Mis Tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) para facilitar la clonación de programas.

1. Seleccione el estado de miembro de campaña de Salesforce que desea asignar a los leads cuando se agreguen.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Si una persona ya es miembro principal de la campaña de Salesforce, se omitirán y NO se actualizará su estado. Puede [cambiar su estado en una campaña](change-status-in-sfdc-campaign.md) SFDC.

