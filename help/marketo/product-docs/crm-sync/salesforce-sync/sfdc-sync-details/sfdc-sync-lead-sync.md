---
unique-page-id: 2953455
description: Sincronización SFDC - Sincronización de posibles clientes - Documentos de Marketo - Documentación del producto
title: 'Sincronización SFDC: Sincronización de posibles clientes'
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Sincronización SFDC: Sincronización de posibles clientes {#sfdc-sync-lead-sync}

¿Sabía que Marketo se sincroniza desde la base de datos de Salesforce? Se sincroniza, espera 5 minutos y luego se sincroniza de nuevo. Todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketo a los posibles clientes de Salesforce de forma específica.

## Dirección de sincronización {#sync-direction}

La sincronización de posibles clientes (personas) y contactos es bidireccional. Si realiza cambios en un registro en Salesforce o Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gana. Es raro que ocurra este tipo de colisión de datos.

## ¿Puedo crear un posible cliente en Salesforce mediante Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sí, utilice la acción de flujo [Sync Person to SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Esto creará un posible cliente en Salesforce si el posible cliente no existe.

## ¿Puedo forzar manualmente la sincronización de una persona en Marketo con un posible cliente en Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sí, utilice la acción de flujo [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) y se sincronizará en tiempo real.

## ¿Se sincroniza cada campo estándar con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo solo sincronizará los campos a los que el usuario de sincronización de Salesforce tenga acceso.

## ¿Marketo respetará las reglas de validación de Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sí. La sincronización fallará si el formato de datos es incorrecto o si falta la información de campo necesaria. Marketo registrará el resultado en el registro de actividades de posibles clientes si esto sucede.
