---
unique-page-id: 2953457
description: Sincronización SFDC - Sincronización de contactos - Documentos de marketing - Documentación del producto
title: Sinc. SFDC - Sinc. contacto
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# Sincronización SFDC: Comuníquese con la sincronización {#sfdc-sync-contact-sync}

¿Sabía que Marketing sincroniza toda la base de datos con Salesforce? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketing a los contactos de Salesforce de forma específica.

## Dirección de sincronización {#sync-direction}

La sincronización de contactos es bidireccional. Si realiza cambios en un contacto de Salesforce o de Marketing, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Somos amables y dejamos que Salesforce gane. Es raro que este tipo de colisión de datos ocurra.

## ¿Puedo convertir una persona en un contacto en Marketing? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sí, utilice la acción de flujo ** [Convertir persona](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**.

>[!CAUTION]
>
>La conversión de una persona en Marketing resultará en una nueva cuenta y oportunidad en Salesforce. Si no desea cuentas de duplicado, utilice Salesforce para convertir.

## ¿Puedo forzar manualmente la sincronización de un contacto? {#can-i-manually-force-a-sync-of-a-contact}

Sí, utilice la acción de flujo ** [Sincronizar persona con SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **y se sincronizará en tiempo real.

## ¿Se sincroniza cada campo estándar con Marketing? {#does-every-single-standard-field-sync-to-marketo}

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo sólo sincronizará los campos a los que tiene acceso el usuario de sincronización de marketing.

## ¿Respetará Marketing las reglas de validación de Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sí, si hay un conflicto, registrará el resultado en el registro de Actividad de posibles clientes.
