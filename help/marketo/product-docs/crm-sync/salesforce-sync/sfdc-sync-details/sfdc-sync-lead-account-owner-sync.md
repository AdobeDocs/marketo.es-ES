---
unique-page-id: 2953463
description: 'Sincronización de SFDC: sincronización de cliente potencial/propietario de cuenta - Documentos de Marketo - Documentación del producto'
title: 'Sincronización de SFDC: sincronización de cliente potencial/Propietario de cuenta'
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 13%

---

# Sincronización de SFDC: sincronización de cliente potencial/propietario de cuenta {#sfdc-sync-lead-account-owner-sync}

Técnicamente, se está sincronizando la tabla &quot;usuario&quot; en Salesforce, pero nos referiremos a ella como campos de Posible cliente/Propietario de cuenta.

## ¿Qué campos se sincronizarán con el Marketo Engage? {#which-fields-will-sync-to-marketo-engage}

Para cada persona sincronizada con Marketo, también sincronizamos los siguientes campos de propietario:

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título de propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de email del propietario de ventas

Para cada contacto, sincronizamos los cinco campos de propietario del posible cliente anteriores, así como estos campos de propietario de la cuenta:

* Nombre del propietario de la cuenta
* Apellido del propietario de la cuenta
* Email del propietario de la cuenta

## ¿Puedo cambiar el propietario del posible cliente en Marketo? {#can-i-change-the-lead-owner-in-marketo}

Por supuesto, solo usa el [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"} acción de flujo.

>[!NOTE]
>
>No puede cambiar la información del propietario mediante el [Uso de la página Detalles de Persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## ¿Qué puedo hacer con estos datos? {#what-can-i-do-with-this-data}

Existen muchas razones para utilizar estos datos, como

* Enviar un correo electrónico personalizado con la firma del propietario de ventas
* Filtre por representantes de ventas específicos para marketing o incluso para analizar la eficacia
* Reglas de asignación (y reasignación) en Marketo
* Utilícelos en el [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Sync Person to SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}, and [Create Task](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} acciones de flujo

Marketo tiene una sincronización de Salesforce increíble. ¡Nadie más lo hace tan bien!
