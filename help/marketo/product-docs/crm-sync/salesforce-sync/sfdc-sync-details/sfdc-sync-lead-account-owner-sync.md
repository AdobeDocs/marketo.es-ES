---
unique-page-id: 2953463
description: Sincronización de SFDC - Sincronización de posibles clientes/propietarios de cuentas - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: Sincronización de posibles clientes y propietarios de cuentas'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Sincronización SFDC: Sincronización del propietario de posibles clientes/cuentas {#sfdc-sync-lead-account-owner-sync}

Técnicamente, están sincronizando la tabla &quot;usuario&quot; en Salesforce, pero se referirán a ella como campos Poseedor de posible cliente/cuenta.

## ¿Qué campos se sincronizarán con Marketing? {#which-fields-will-sync-to-marketo}

Para cada persona sincronizada con Marketing, también se sincronizan los siguientes campos de propietario:

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título del propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de correo electrónico del propietario de ventas

Para cada contacto, sincronizamos los cinco campos de propietario de posibles clientes anteriores, así como los campos de propietario de la cuenta siguientes:

* Nombre del propietario de la cuenta
* Apellido del propietario de la cuenta
* Dirección de correo electrónico del propietario de la cuenta

## ¿Puedo cambiar el propietario principal en Marketing? {#can-i-change-the-lead-owner-in-marketo}

Absolutamente, simplemente utilice la acción de flujo [Cambiar propietario](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>No se puede cambiar la información del propietario mediante [Uso de la página de detalles de la persona](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## ¿Qué puedo hacer con estos datos? {#what-can-i-do-with-this-data}

Existen muchas razones para utilizar estos datos, como

* Enviar un correo electrónico personalizado con la firma del propietario de ventas
* Filtrar en determinados representantes de ventas para marketing o incluso analizar la eficacia
* Reglas de asignación (y reasignación) en Marketing
* Utilícelos en las acciones de flujo [Cambiar propietario](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizar persona a SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) y [Crear Tarea](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)

Marketo seguro tiene una asombrosa sincronización de Salesforce. ¡Nadie lo hace tan bien!
