---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Sincronización de campos - Documentos de marketing - Documentación del producto
title: Sincronización de Microsoft Dynamics - Sincronización de campos
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronización de campos {#microsoft-dynamics-sync-field-sync}

La sincronización de marketing a Dynamics es muy potente. Aquí están los detalles.

## ¿Cómo se mantienen sincronizados los detalles de campo entre los dos sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional para entidades de contacto y posibles clientes. Si realiza cambios en un posible cliente o contacto en Dynamics o en una persona de Marketing, las actualizaciones se reflejarán en ambos sistemas.

Para las entidades de cuenta, usuario, oportunidad, equipo y personalizadas, la sincronización es unidireccional: Dinámica a Marketing. Si realiza cambios en estas entidades en Dynamics, las actualizaciones se reflejarán en Marketing.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Colisión de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto es raro, Marketo ganará para las personas (posibles clientes) y Dynamics ganará para los contactos. Esto se debe a que consideramos que el departamento de mercadotecnia tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos está en el departamento de ventas (CRM). Para las entidades de sincronización unidireccional, Dynamics siempre ganará.

## ¿Puedo crear un campo en Dynamics con Marketing? {#can-i-create-a-field-in-dynamics-using-marketo}

No, no se admite actualmente.

## He creado un campo en Dynamics. ¿Puedo sincronizarlo con Marketing? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sí, puede [sincronizar el campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) siempre y cuando el usuario de sincronización tenga acceso a él en Dynamics.

¿Qué campos se sincronizarán con Marketing?

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configuración.

## ¿Qué sucede si necesito agregar un campo personalizado después de sincronizar Marketing y Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puede agregar campos en cualquier momento y esperar que los datos se actualicen de Dynamics a Marketing. Consulte [Usar sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) para obtener más información.
