---
unique-page-id: 2953461
description: 'Sincronización de SFDC: sincronización de campos, documentos de Marketo, documentación del producto'
title: 'Sincronización de SFDC: sincronización de campos'
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Sincronización de SFDC: sincronización de campos {#sfdc-sync-field-sync}

Marketo sincroniza la información de campo de [!DNL Salesforce]. Aquí están los detalles.

## ¿Qué campos se sincronizan? {#which-fields-are-synced}

Sincronizamos la mayoría de los campos estándar en SFDC y cualquier campo personalizado que el usuario de sincronización tenga permiso para ver.

## ¿Cómo determina si un registro en Marketo es un posible cliente o un contacto en [!DNL Salesforce]? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Tenemos un campo en Marketo llamado Tipo de SFDC. Tiene tres valores posibles: posible cliente, contacto o si está vacío. Si está vacío, significa que este posible cliente de Marketo no existe en SFDC.

## ¿Cómo determina si un posible cliente o contacto se elimina en SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Tenemos un campo en Marketo llamado SFDC isDeleted. Si el valor es True, el posible cliente se eliminó en SFDC.

## ¿Cómo me aseguro de que un nuevo campo que añado en SFDC también se añada a Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Si desea un campo en ambos sistemas, créelo primero en SFDC y se sincronizará automáticamente con Marketo.

Si agrega un nuevo campo en SFDC y el usuario de sincronización tiene permiso para verlo, se agregará automáticamente a Marketo.

## ¿Qué sucede si cambio una etiqueta de campo en SFDC? {#what-if-i-change-a-field-label-in-sfdc}

Cambiar la etiqueta del campo en SFDC no afecta a la etiqueta del campo en Marketo.

## ¿Qué sucede si cambio un tipo de campo en SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Al cambiar un tipo de campo, Marketo elimina los datos de los campos si no coinciden (pero primero muestra una advertencia). Para conservar los datos, asegúrese de exportarlos y volver a importarlos después de cambiar el tipo de campo.

## ¿Qué sucede si cambio el nombre de una API en SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Si cambia el nombre de la API de un campo en SFDC, se crea un nuevo campo en Marketo.

## ¿Qué sucede si añado un nuevo valor de lista de selección en SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Si se añade un nuevo valor de lista de selección en SFDC a un campo, Marketo le enviará una notificación.

## ¿Qué sucede con los campos de búsqueda personalizados de SFDC? {#what-about-custom-sfdc-lookup-fields}

Los campos de búsqueda en SFDC sincronizan el ID, pero no el nombre al que se hace referencia.

## ¿Qué sucede con los campos de fórmula de SFDC? {#what-about-sfdc-formula-fields}

Los campos de fórmula están sincronizados, sin embargo, las actualizaciones de las referencias en la fórmula no se sincronizarán hasta que se actualice [System Mod Stamp](https://help.salesforce.com/apex/HTViewSolution?id=000193203&language=en_US){target="_blank"}.

## ¿Qué sucede cuando elimino un campo de [!DNL Salesforce] que se estaba sincronizando anteriormente con Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Si elimina un campo en SFDC, no se elimina automáticamente en Marketo, solo se detiene la sincronización.
