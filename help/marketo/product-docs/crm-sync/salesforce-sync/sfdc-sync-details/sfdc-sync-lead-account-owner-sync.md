---
unique-page-id: 2953463
description: Sincronización SFDC - Sincronización de posibles clientes/propietarios de cuentas - Documentos de Marketo - Documentación del producto
title: 'Sincronización SFDC: Sincronización de posibles clientes/propietarios de cuentas'
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Sincronización SFDC: Sincronización de posibles clientes/propietarios de cuentas {#sfdc-sync-lead-account-owner-sync}

Técnicamente, están sincronizando la tabla &quot;usuario&quot; en Salesforce, pero nos referiremos a ella como campos Propietario de posibles clientes o cuentas.

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Para cada persona sincronizada con Marketo, también sincronizamos los siguientes campos de propietario:

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título del propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de correo electrónico del propietario de ventas

Para cada contacto, sincronizamos los cinco campos de propietario de posibles clientes anteriores, así como los campos de propietario de la cuenta:

* Nombre del propietario de la cuenta
* Apellido del propietario de la cuenta
* Dirección de correo electrónico del propietario de la cuenta

## ¿Puedo cambiar el propietario del posible cliente en Marketo? {#can-i-change-the-lead-owner-in-marketo}

Absolutamente, utilice la acción de flujo [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>No se puede cambiar la información de propietario mediante [Uso de la página de detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## ¿Qué puedo hacer con estos datos? {#what-can-i-do-with-this-data}

Existen muchas razones para utilizar estos datos, como

* Enviar un correo electrónico personalizado con la firma del propietario de ventas
* Filtrar por representantes de ventas específicos para marketing o incluso analizar la eficacia
* Reglas de asignación (y reasignación) en Marketo
* Utilícelos en las acciones de flujo [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizar persona a SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) y [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)

Marketo tiene una sincronización impresionante de Salesforce. ¡Nadie lo hace tan bien!
