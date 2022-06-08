---
unique-page-id: 2953463
description: Sincronización SFDC - Sincronización de posibles clientes/propietarios de cuentas - Documentos de Marketo - Documentación del producto
title: 'Sincronización SFDC: Sincronización de posibles clientes/propietarios de cuentas'
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 13%

---

# Sincronización SFDC: Sincronización de posibles clientes/propietarios de cuentas {#sfdc-sync-lead-account-owner-sync}

Técnicamente, están sincronizando la tabla &quot;usuario&quot; en Salesforce, pero nos referiremos a ella como campos Propietario de posibles clientes o cuentas.

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Para cada persona sincronizada con Marketo, también sincronizamos los siguientes campos de propietario:

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título del propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de email del propietario de ventas

Para cada contacto, sincronizamos los cinco campos de propietario de posibles clientes anteriores, así como los campos de propietario de la cuenta:

* Nombre del propietario de la cuenta
* Apellido del propietario de la cuenta
* Email del propietario de la cuenta

## ¿Puedo cambiar el propietario del posible cliente en Marketo? {#can-i-change-the-lead-owner-in-marketo}

Por supuesto, use el [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) acción de flujo.

>[!NOTE]
>
>No se puede cambiar la información de propietario utilizando la variable [Uso de la página de detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## ¿Qué puedo hacer con estos datos? {#what-can-i-do-with-this-data}

Existen muchas razones para utilizar estos datos, como

* Enviar un correo electrónico personalizado con la firma del propietario de ventas
* Filtrar por representantes de ventas específicos para marketing o incluso analizar la eficacia
* Reglas de asignación (y reasignación) en Marketo
* Utilícelos en el [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)y [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) acciones de flujo

Marketo tiene una sincronización impresionante de Salesforce. ¡Nadie lo hace tan bien!
