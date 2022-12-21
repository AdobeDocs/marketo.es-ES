---
unique-page-id: 2953461
description: Sincronización SFDC - Sincronización de campos - Documentos de Marketo - Documentación del producto
title: Sincronización SFDC - Sincronización de campos
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Sincronización SFDC: Sincronización de campos {#sfdc-sync-field-sync}

Marketo sincroniza la información de campo de Salesforce. Aquí están los detalles.

## ¿Qué campos se sincronizan? {#which-fields-are-synced}

Sincronizamos la mayoría de los campos estándar en SFDC y cualquier campo personalizado que el usuario de sincronización tenga permiso para ver.

## ¿Cómo determina si un registro en Marketo es un posible cliente o un contacto en Salesforce? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Tenemos un campo en Marketo llamado Tipo de SFDC. Tiene tres valores posibles: posible cliente, contacto o está vacío. Si está vacío, significa que este posible cliente de Marketo no existe en SFDC.

## ¿Cómo determina si un posible cliente o contacto se elimina en SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Tenemos un campo en Marketo llamado SFDC isDeleted. Si el valor es true, el posible cliente se eliminó en SFDC.

## ¿Cómo puedo asegurarme de que un nuevo campo que añado en SFDC también se añada a Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Si desea un campo en ambos sistemas, créelo primero en SFDC y se sincronizará automáticamente con Marketo.

Si agrega un nuevo campo en SFDC y el usuario de sincronización tiene permiso para verlo, se agregará automáticamente a Marketo.

## ¿Qué sucede si cambio una etiqueta de campo en SFDC? {#what-if-i-change-a-field-label-in-sfdc}

Cambiar la etiqueta de campo en SFDC no afecta a la etiqueta de campo en Marketo.

## ¿Qué sucede si cambio un tipo de campo en SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Al cambiar un tipo de campo, Marketo elimina los datos de los campos si no coinciden (pero primero muestra una advertencia). Para conservar los datos, asegúrese de exportarlos y volver a importarlos después de cambiar el tipo de campo.

## ¿Qué sucede si cambio un nombre de API en SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Si cambia el nombre de la API de un campo en SFDC, se crea un nuevo campo en Marketo.

## ¿Qué sucede si añado un nuevo valor de lista de selección en SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Si se agrega un nuevo valor de lista de selección en SFDC a un campo, Marketo le enviará una notificación.

## ¿Qué sucede con los campos de búsqueda de SFDC personalizados? {#what-about-custom-sfdc-lookup-fields}

Los campos de búsqueda en SFDC sincronizan el ID, pero no el nombre al que se hace referencia.

## ¿Qué sucede con los campos de fórmula de SFDC? {#what-about-sfdc-formula-fields}

Los campos de fórmula se sincronizan, sin embargo, las actualizaciones de las referencias de la fórmula no se sincronizan hasta que haya una actualización de [Sello de Mod del sistema](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## ¿Qué sucede cuando elimino un campo de Salesforce que anteriormente se sincronizaba con Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Si elimina un campo en SFDC, no elimina automáticamente el campo en Marketo, solo detiene la sincronización.
