---
unique-page-id: 2953461
description: Sincronización de SFDC - Sincronización de campos - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: sincronización de campos'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# Sincronización SFDC: Sincronización de campos {#sfdc-sync-field-sync}

Marketo sincroniza la información de campo de Salesforce. Aquí están los detalles.

## ¿Qué campos se sincronizan? {#which-fields-are-synced}

Sincronizamos la mayoría de los campos estándar en SFDC y todos los campos personalizados que el usuario de sincronización tenga permiso para ver.

## ¿Cómo determina si un registro en Marketing es un posible cliente o un contacto en Salesforce? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Tenemos un campo en Marketing llamado Tipo SFDC. Tiene tres valores posibles: posible cliente, contacto o está vacío. Si está vacío, significa que este posible cliente de marketing no existe en SFDC.

## ¿Cómo determina si un posible cliente o contacto se elimina en SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Tenemos un campo en Marketing llamado SFDC isDeleted. Si el valor es true, el lead se eliminó en SFDC.

## ¿Cómo puedo asegurarme de que un nuevo campo que añado en SFDC también se añada a Marketing? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Si desea un campo en ambos sistemas, primero debe crearlo en SFDC y se sincronizará automáticamente con Marketing.

Si agrega un nuevo campo en SFDC y el usuario de sincronización tiene permiso para verlo, automáticamente se agregará a Marketing.

## ¿Qué sucede si cambio una etiqueta de campo en SFDC? {#what-if-i-change-a-field-label-in-sfdc}

El cambio de la etiqueta de campo en SFDC no afecta a la etiqueta de campo en Marketing.

## ¿Qué sucede si cambio un tipo de campo en SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Al cambiar un tipo de campo, Marketo elimina los datos de los campos si no coinciden (pero primero muestra una advertencia). Para conservar los datos, asegúrese de exportarlos y volver a importarlos después de cambiar el tipo de campo.

## ¿Qué sucede si cambio un nombre de API en SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Si cambia el nombre de la API de un campo en SFDC, se crea un nuevo campo en Marketing.

## ¿Qué sucede si agrego un nuevo valor de lista de selección en SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Si se agrega un nuevo valor de lista de selección en SFDC a un campo, Marketing le enviará una notificación.

## ¿Qué sucede con los campos de búsqueda personalizados de SFDC? {#what-about-custom-sfdc-lookup-fields}

Los campos de búsqueda en SFDC sincronizan el ID pero no el nombre al que se hace referencia.

## ¿Qué sucede con los campos de fórmula de SFDC? {#what-about-sfdc-formula-fields}

Los campos de fórmula se sincronizan, sin embargo, las actualizaciones de las referencias de la fórmula no se sincronizan hasta que haya una actualización de [Marca de método del sistema](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## ¿Qué sucede cuando elimino un campo de Salesforce que se sincronizaba previamente con Marketing? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Si elimina un campo en SFDC, no se elimina automáticamente el campo en Marketo, solo se detiene la sincronización.
