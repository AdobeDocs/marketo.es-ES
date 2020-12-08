---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Sincronización de posibles clientes - Documentos de marketing - Documentación del producto
title: 'Microsoft Dynamics Sync: sincronización de posibles clientes'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronización de posibles clientes {#microsoft-dynamics-sync-lead-sync}

La sincronización de marketing a Dynamics es muy potente. A continuación se detallan los detalles:

## ¿Cómo se mantienen los detalles sincronizados entre los dos sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional. Si realiza cambios en un posible cliente de Dynamics o en una persona de Marketing, la actualización se verá reflejada en ambos sistemas.

>[!NOTE]
>
>Las eliminaciones no siempre se sincronizan automáticamente en ambas direcciones. Consulte [Eliminación de un posible cliente o contacto](http://docs.marketo.com/x/agO1Ag).

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Colisión de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto es raro, Marketo ganará para las personas (posibles clientes) y Dynamics ganará para los contactos. Esto se debe a que consideramos que el departamento de mercadotecnia tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos está en el departamento de ventas (CRM).

## ¿Puedo crear un lead en Dynamics con Marketing? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sí, utilice la acción de flujo [Sincronizar persona con Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) . Esto creará un posible cliente en Dynamics si el posible cliente no existe. Si el lead existe, el paso de flujo no realizará ninguna acción.

>[!NOTE]
>
>Al utilizar la acción de flujo &quot;Sincronizar persona con Microsoft&quot; (solo en una campaña desencadenadora), el posible cliente o contacto se creará en tiempo real en Dynamics.

## ¿Puedo forzar manualmente la sincronización de una persona de Marketing a un posible cliente en Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

No, la sincronización en segundo plano automatizada es la única manera de sincronizar las actualizaciones entre Marketing y Dynamics. La acción de flujo [Sincronizar persona con Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) no fuerza la sincronización del posible cliente.

## ¿Qué campos se sincronizarán con Marketing? {#what-fields-will-sync-to-marketo}

Puede [seleccionar los campos que sincronizar](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante la configuración.

## ¿Respetará Marketing las reglas de validación de Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sí. La sincronización fallará si el formato de datos es incorrecto o si falta la información de campo requerida. Marketo registrará el resultado en el registro de Actividad de la persona si esto sucede.

