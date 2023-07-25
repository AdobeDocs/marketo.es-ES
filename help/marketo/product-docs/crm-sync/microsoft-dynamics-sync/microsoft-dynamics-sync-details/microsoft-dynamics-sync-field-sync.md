---
unique-page-id: 3571838
description: 'Sincronización de Microsoft Dynamics: sincronización de campos - Documentos de Marketo: documentación del producto'
title: 'Sincronización de Microsoft Dynamics: sincronización de campos'
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Sincronización de Microsoft Dynamics: sincronización de campos {#microsoft-dynamics-sync-field-sync}

La sincronización de Marketo con Dynamics es muy potente. Aquí están los detalles.

## ¿Cómo se sincronizan los detalles de campo entre los dos sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional para entidades de contacto y posible cliente. Si realiza cambios en un posible cliente o contacto en Dynamics o en una persona en Marketo, las actualizaciones se reflejarán en ambos sistemas.

Para entidades de cuenta, usuario, oportunidad, equipo y personalizadas, la sincronización es unidireccional: de Dynamics a Marketo. Si realiza cambios en estas entidades en Dynamics, las actualizaciones se reflejarán en Marketo.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Conflicto de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto no es habitual, Marketo ganará para las personas (posibles clientes) y Dynamics para los contactos. Esto se debe a que consideramos que el departamento de marketing tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos se encuentra en el departamento de ventas (CRM). Para entidades de sincronización unidireccionales, Dynamics siempre gana.

## ¿Puedo crear un campo en Dynamics con Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, actualmente no es compatible.

## He creado un campo en Dynamics. ¿Puedo sincronizarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sí, puede [sincronizar el campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) siempre que el usuario de sincronización tenga acceso a él en Dynamics.

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante la configuración.

## ¿Qué sucede si necesito agregar un campo personalizado después de sincronizar Marketo y Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puede agregar campos en cualquier momento y esperar que los datos se actualicen de Dynamics a Marketo. Consulte [Usar la sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) para obtener más información.

## ¿Qué sucede si deseo eliminar un campo en Dynamics después de agregar el campo para sincronizarlo? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo en Dynamics, se recomienda hacerlo con la variable [sincronización deshabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). A continuación, actualice el esquema en Marketo editando y guardando el [Seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
