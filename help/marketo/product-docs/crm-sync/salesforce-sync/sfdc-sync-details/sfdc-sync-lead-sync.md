---
unique-page-id: 2953455
description: Sincronización de SFDC - Sincronización de posibles clientes - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: sincronización de posibles clientes'
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# Sincronización SFDC: Sincronización de posibles clientes {#sfdc-sync-lead-sync}

¿Sabía que Marketing se sincroniza desde la base de datos de Salesforce? Se sincroniza, espera 5 minutos y luego se sincroniza nuevamente. Todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketing a los posibles clientes de Salesforce de forma específica.

## Dirección de sincronización {#sync-direction}

La sincronización de contactos y posibles clientes es bidireccional. Si realiza cambios en un registro en Salesforce o Marketing, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

El comerciante gana. Es raro que este tipo de colisión de datos ocurra.

## ¿Puedo crear un posible cliente en Salesforce mediante Marketing? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sí, utilice la acción de flujo [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Esto creará un posible cliente en Salesforce si el posible cliente no existe.

## ¿Puedo forzar manualmente la sincronización de una persona en Marketing con un posible cliente en Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sí, utilice la acción de flujo [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) y se sincronizará en tiempo real.

## ¿Se sincroniza cada campo estándar con Marketing? {#does-every-single-standard-field-sync-to-marketo}

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo sólo sincronizará los campos a los que tiene acceso el usuario de sincronización de Salesforce.

## ¿Respetará Marketing las reglas de validación de Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sí. La sincronización fallará si el formato de datos es incorrecto o si falta la información de campo requerida. Marketo registrará el resultado en el registro de Actividad de posibles clientes si esto sucede.
