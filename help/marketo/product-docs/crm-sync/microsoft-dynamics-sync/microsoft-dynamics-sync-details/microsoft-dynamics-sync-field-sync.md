---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Sincronización de campos - Documentos de Marketo - Documentación del producto
title: Sincronización de Microsoft Dynamics - Sincronización de campos
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronización de campos {#microsoft-dynamics-sync-field-sync}

La sincronización entre Marketo y Dynamics es superpotente. Aquí están los detalles.

## ¿Cómo se mantienen los detalles de campo sincronizados entre los dos sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional para entidades de contacto y posibles clientes. Si realiza cambios en un posible cliente o contacto en Dynamics o en una persona de Marketo, las actualizaciones se reflejarán en ambos sistemas.

Para la cuenta, el usuario, la oportunidad, el equipo y las entidades personalizadas, la sincronización es unidireccional: Dynamics a Marketo. Si realiza cambios en estas entidades en Dynamics, las actualizaciones se reflejarán en Marketo.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Conflicto de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto es poco frecuente, Marketo ganará para las personas (posibles clientes) y Dynamics ganará para los contactos. Esto se debe a que consideramos que el departamento de marketing es autorizado para las personas, mientras que el sistema oficial de registro de contactos está en el departamento de ventas (CRM). Para las entidades de sincronización unidireccional, Dynamics siempre ganará.

## ¿Puedo crear un campo en Dynamics con Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, actualmente no es compatible.

## He creado un campo en Dynamics. ¿Puedo sincronizarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sí, puede [sincronizar el campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) siempre que el usuario de sincronización tenga acceso a él en Dynamics.

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configuración.

## ¿Qué sucede si necesito agregar un campo personalizado después de sincronizar Marketo y Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puede agregar campos en cualquier momento y esperar que los datos se actualicen de Dynamics a Marketo. Consulte [Uso de la sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) para obtener más información.

## ¿Qué sucede si deseo eliminar un campo en Dynamics después de agregar el campo para sincronizar? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo en Dynamics, se recomienda hacerlo con la [sincronización deshabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). A continuación, actualice el esquema en Marketo editando y guardando el [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
