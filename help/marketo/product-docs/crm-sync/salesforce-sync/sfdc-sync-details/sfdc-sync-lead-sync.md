---
unique-page-id: 2953455
description: 'Sincronización de SFDC: sincronización de posibles clientes - Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: sincronización de posibles clientes'
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Sincronización de SFDC: sincronización de posibles clientes {#sfdc-sync-lead-sync}

¿Sabía que Marketo sincroniza desde su base de datos [!DNL Salesforce]? Se sincroniza, espera 5 minutos y luego se sincroniza de nuevo. Todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo Marketo trata específicamente los posibles clientes de [!DNL Salesforce].

## Dirección de sincronización {#sync-direction}

La sincronización de posible cliente (persona) y contacto es bidireccional. Si realiza cambios en un registro en [!DNL Salesforce] o Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gana. Es raro que ocurra este tipo de colisión de datos.

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
