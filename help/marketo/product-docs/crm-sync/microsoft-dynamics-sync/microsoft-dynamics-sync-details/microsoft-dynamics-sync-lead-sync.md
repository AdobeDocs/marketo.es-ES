---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Sincronización de posibles clientes - Documentos de Marketo - Documentación del producto
title: 'Microsoft Dynamics Sync: Sincronización de posibles clientes'
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
source-git-commit: 7fcbaeda589682fdb5a75b89a0abd8661181566e
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronización de posibles clientes {#microsoft-dynamics-sync-lead-sync}

La sincronización entre Marketo y Dynamics es superpotente. Aquí están los detalles:

## ¿Cómo se mantienen los detalles sincronizados entre los dos sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional. Si realiza cambios en un posible cliente en Dynamics o en una persona en Marketo, la actualización se reflejará en ambos sistemas.

>[!NOTE]
>
>Las eliminaciones no siempre se sincronizan automáticamente en ambas direcciones. Consulte [Eliminación de un posible cliente o contacto](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Conflicto de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto no es habitual, Marketo ganará para las personas (posibles clientes) y Dynamics ganará para los contactos. Esto se debe a que consideramos que el departamento de marketing es autorizado para las personas, mientras que el sistema oficial de registro de contactos está en el departamento de ventas (CRM).

## ¿Puedo crear un posible cliente en Dynamics con Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sí, use la variable [Sincronizar persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) acción de flujo. Esto creará un posible cliente en Dynamics si el posible cliente no existe. Si el posible cliente existe, el paso de flujo no realiza ninguna acción.

>[!NOTE]
>
>Al utilizar la acción de flujo &quot;Sincronizar persona con Microsoft&quot; (solo en una campaña de déclencheur), el posible cliente o contacto se creará en tiempo real en Dynamics.

## ¿Puedo forzar manualmente la sincronización de una persona de Marketo a un posible cliente en Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

No, la sincronización en segundo plano automatizada es la única forma de sincronizar las actualizaciones entre Marketo y Dynamics. La variable [Sincronizar persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) la acción de flujo no fuerza una sincronización del posible cliente.

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante la configuración.

## ¿Marketo respetará las reglas de validación de Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sí. La sincronización fallará si el formato de datos es incorrecto o si falta la información de campo necesaria. Marketo registrará el resultado en el registro de actividades de la persona si esto sucede.
