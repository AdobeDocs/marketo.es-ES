---
unique-page-id: 2953457
description: 'Sincronización de SFDC: sincronización de contactos - Documentos de Marketo - Documentación del producto'
title: 'Sincronización SFDC: sincronización de contactos'
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Sincronización SFDC: sincronización de contactos {#sfdc-sync-contact-sync}

¿Sabía que Marketo Engage sincroniza toda su base de datos con Salesforce? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación, se muestran algunos detalles sobre cómo Marketo trata a los contactos de Salesforce específicamente.

## Dirección de sincronización {#sync-direction}

La sincronización de contactos es bidireccional. Si realiza cambios en un contacto en Salesforce o Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Somos amables y dejamos que Salesforce gane. Es raro que ocurra este tipo de colisión de datos.

## ¿Puedo convertir a una persona en un contacto en Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sí, usar la acción de flujo **[Convertir persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>Convertir a una persona en Marketo resultará en una nueva cuenta y oportunidad en Salesforce. Si no desea cuentas duplicadas, utilice Salesforce para convertir.

## ¿Puedo forzar manualmente una sincronización de un contacto? {#can-i-manually-force-a-sync-of-a-contact}

Sí, usar la acción de flujo **[Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** y se sincronizará en tiempo real.

## ¿Se sincronizan todos y cada uno de los campos estándar con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo solo sincronizará los campos a los que el usuario de sincronización de Marketo tenga acceso.

## ¿Marketo respetará las reglas de validación de Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sí, si hay un conflicto, registrará el resultado en el registro de actividad de posibles clientes.
