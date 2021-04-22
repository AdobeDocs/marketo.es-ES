---
unique-page-id: 2953457
description: Sincronización SFDC - Sincronización de contactos - Documentos de Marketo - Documentación del producto
title: Sincronización SFDC - Sincronización de contactos
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Sincronización SFDC: Sincronización de contactos {#sfdc-sync-contact-sync}

¿Sabía que Marketo sincroniza toda la base de datos con Salesforce? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketo específicamente a los contactos de Salesforce.

## Dirección de sincronización {#sync-direction}

La sincronización de contactos es bidireccional. Si realiza cambios en un contacto en Salesforce o Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Somos buenos y dejamos que Salesforce gane. Es raro que ocurra este tipo de colisión de datos.

## ¿Puedo convertir una persona en un contacto en Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sí, utilice la acción de flujo **[Convertir persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**.

>[!CAUTION]
>
>La conversión de una persona en Marketo dará como resultado una nueva cuenta y una nueva oportunidad en Salesforce. Si no desea cuentas duplicadas, utilice Salesforce para convertir.

## ¿Puedo forzar manualmente la sincronización de un contacto? {#can-i-manually-force-a-sync-of-a-contact}

Sí, utilice la acción de flujo **[Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** y se sincronizará en tiempo real.

## ¿Se sincroniza cada campo estándar con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo solo sincronizará los campos a los que el usuario de sincronización de Marketo tenga acceso.

## ¿Marketo respetará las reglas de validación de Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sí, si hay un conflicto, registrará el resultado en el registro de actividades de posibles clientes.
