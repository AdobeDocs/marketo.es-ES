---
unique-page-id: 3571833
description: Microsoft Dynamics Sync - Sincronización de contactos - Documentos de Marketo - Documentación del producto
title: 'Microsoft Dynamics Sync: Sincronización de contactos'
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronización de contactos {#microsoft-dynamics-sync-contact-sync}

¿Sabía que Marketo sincroniza toda la base de datos con Dynamics? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketo específicamente a los contactos de Dynamics.

## ¿Cómo se mantienen los detalles sincronizados entre los dos sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronización de contactos es bidireccional. Si realiza cambios en un contacto de Dynamics o en una persona de Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Conflicto de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto es raro, Marketo ganará para las personas y Dynamics ganará para los contactos. Esto se debe a que consideramos que el departamento de marketing es autorizado para las personas, mientras que el sistema oficial de registro de contactos está en el departamento de ventas (CRM).

## ¿Puedo crear un contacto con Marketo? {#can-i-create-a-contact-using-marketo}

Sí. [Así es como](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>Al utilizar la acción de flujo &quot;Sincronizar persona con Microsoft&quot; (solo en una campaña de déclencheur), el posible cliente o contacto se creará en tiempo real en Dynamics.

## ¿Puedo forzar manualmente la sincronización de una persona o un contacto? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

No, la sincronización en segundo plano automatizada es la única forma de sincronizar las actualizaciones entre Marketo y Dynamics. La variable [Sincronizar persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) no fuerza una sincronización del posible cliente.

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) durante la configuración. Sin embargo, Marketo solo sincronizará los campos a los que el usuario de sincronización con Dynamics tiene acceso.

## ¿Marketo respetará las reglas de validación de Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sí, si hay un conflicto, registrará el resultado en el registro de actividades de posibles clientes.
