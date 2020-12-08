---
unique-page-id: 3571833
description: Microsoft Dynamics Sync - Sincronización de contactos - Documentos de marketing - Documentación del producto
title: Microsoft Dynamics Sync - Sincronización de contactos
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronización de contactos {#microsoft-dynamics-sync-contact-sync}

¿Sabía que Marketing sincroniza toda la base de datos con Dynamics? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketing a los contactos de Dynamics de forma específica.

## ¿Cómo se mantienen los detalles sincronizados entre los dos sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronización de contactos es bidireccional. Si realiza cambios en un contacto de Dynamics o en una persona de Marketing, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Colisión de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto es raro, Marketo ganará para las personas y Dynamics ganará para los contactos. Esto se debe a que consideramos que el departamento de mercadotecnia tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos está en el departamento de ventas (CRM).

## ¿Puedo crear un contacto con Marketing? {#can-i-create-a-contact-using-marketo}

Sí. [Así es como](microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>Al utilizar la acción de flujo &quot;Sincronizar persona con Microsoft&quot; (solo en una campaña desencadenadora), el posible cliente o contacto se creará en tiempo real en Dynamics.

## ¿Puedo forzar manualmente la sincronización de una persona o un contacto? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

No, la sincronización en segundo plano automatizada es la única manera de sincronizar las actualizaciones entre Marketing y Dynamics. La [sincronización de persona con Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) no forzará la sincronización del posible cliente.

## ¿Qué campos se sincronizarán con Marketing? {#what-fields-will-sync-to-marketo}

Puede [seleccionar los campos que sincronizar](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante la configuración. Sin embargo, Marketing solo sincronizará los campos a los que tiene acceso el usuario de sincronización de Dynamics.

## ¿Respetará Marketing las reglas de validación de Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sí, si hay un conflicto, registrará el resultado en el registro de Actividad de posibles clientes.
