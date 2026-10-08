---
unique-page-id: 2953455
description: Obtenga información acerca de cómo funciona la sincronización de posibles clientes entre Salesforce y Marketo. Comprenda la sincronización bidireccional, cree posibles clientes a partir de Marketo y respete las reglas de validación.
title: 'Sincronización de SFDC: sincronización de posibles clientes'
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/zqztwtX4Xe08Df-v1aTxhRi-cB2CZALctr3kaFNrT7s'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 2%
---
# Sincronización de SFDC: sincronización de posibles clientes {#sfdc-sync-lead-sync}

Marketo sincroniza desde su base de datos [!DNL Salesforce]. Se sincroniza, espera 5 minutos y luego se sincroniza de nuevo. Todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo Marketo trata específicamente los posibles clientes de [!DNL Salesforce].

## Dirección de sincronización {#sync-direction}

La sincronización de posible cliente (persona) y contacto es bidireccional. Si realiza cambios en un registro en [!DNL Salesforce] o Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gana. Es poco frecuente que se produzca este tipo de colisión de datos.

## ¿Puedo crear un posible cliente en [!DNL Salesforce] mediante Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sí, usar la acción de flujo [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Esto creará un posible cliente en [!DNL Salesforce] si el posible cliente no existe.

## ¿Puedo forzar manualmente una sincronización de una persona en Marketo con un posible cliente en [!DNL Salesforce]? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sí, usar la acción de flujo [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} y se sincronizará en tiempo real.

## ¿Se sincronizan todos y cada uno de los campos estándar con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo solo sincronizará los campos a los que el usuario de sincronización [!DNL Salesforce] tenga acceso.

## ¿Marketo respetará las reglas de validación de [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Sí. La sincronización fallará si el formato de datos es incorrecto o si falta información de campo necesaria. Marketo registrará el resultado en el registro de actividades de posibles clientes si esto sucede.
