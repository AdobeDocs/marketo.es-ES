---
unique-page-id: 3571838
description: 'Sincronización de Microsoft Dynamics: sincronización de campos - Documentos de Marketo: documentación del producto'
title: 'Sincronización de Microsoft Dynamics: sincronización de campos'
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Sincronización de [!DNL Microsoft Dynamics]: sincronización de campos {#microsoft-dynamics-sync-field-sync}

La sincronización de Marketo con [!DNL Dynamics] es muy eficaz. Aquí están los detalles.

## ¿Cómo se sincronizan los detalles de campo entre los dos sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional para entidades de contacto y posible cliente. Si realiza cambios en un posible cliente o contacto de [!DNL Dynamics] o en una persona de Marketo, las actualizaciones se reflejarán en ambos sistemas.

Para entidades de cuenta, usuario, oportunidad, equipo y personalizadas, la sincronización es unidireccional: [!DNL Dynamics] con Marketo. Si realiza cambios en estas entidades en [!DNL Dynamics], las actualizaciones se reflejarán en Marketo.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Conflicto de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque no es habitual, Marketo ganará para las personas (posibles clientes) y [!DNL Dynamics] para los contactos. Esto se debe a que consideramos que el departamento de marketing tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos se encuentra en el departamento de ventas (CRM). Para entidades de sincronización unidireccional, [!DNL Dynamics] siempre ganará.

## ¿Puedo crear un campo en [!DNL Dynamics] mediante Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

No, actualmente no es compatible.

## Creé un campo en [!DNL Dynamics]. ¿Puedo sincronizarlo con Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sí, puede [sincronizar el campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) siempre y cuando su usuario de sincronización tenga acceso a él en [!DNL Dynamics].

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante la instalación.

## ¿Qué sucede si necesito agregar un campo personalizado después de sincronizar Marketo y [!DNL Dynamics]? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puede agregar campos en cualquier momento y esperar que los datos se actualicen de [!DNL Dynamics] a Marketo. Consulte [Usar sincronización rápida con [!DNL Microsoft Dynamics] para un nuevo campo personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) para obtener más información.

## ¿Qué sucede si deseo eliminar un campo de [!DNL Dynamics] después de que el campo se haya agregado a la sincronización? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo almacena una referencia a los campos que se van a sincronizar. Si elimina un campo de [!DNL Dynamics], se recomienda hacerlo con la [sincronización deshabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). A continuación, actualice el esquema en Marketo editando y guardando [Seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
