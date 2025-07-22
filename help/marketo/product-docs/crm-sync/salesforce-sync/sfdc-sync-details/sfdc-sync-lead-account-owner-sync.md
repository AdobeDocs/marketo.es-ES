---
unique-page-id: 2953463
description: 'Sincronización de SFDC: sincronización de cliente potencial/propietario de cuenta - Documentos de Marketo - Documentación del producto'
title: 'Sincronización de SFDC: sincronización de cliente potencial/Propietario de cuenta'
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 13%

---

# Sincronización de SFDC: sincronización de cliente potencial/Propietario de cuenta {#sfdc-sync-lead-account-owner-sync}

Técnicamente están sincronizando la tabla &quot;usuario&quot; en [!DNL Salesforce], sin embargo, nos referiremos a ella como campos Propietario de cliente potencial/Cuenta.

## ¿Qué campos se sincronizarán con Marketo Engage? {#which-fields-will-sync-to-marketo-engage}

Para cada persona sincronizada con Marketo, también sincronizamos los siguientes campos de propietario:

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título de propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de correo electrónico del propietario de ventas

Para cada contacto, sincronizamos los cinco campos de propietario del posible cliente anteriores, así como estos campos de propietario de la cuenta:

* Nombre del propietario de la cuenta
* Apellido del propietario de la cuenta
* Email del propietario de la cuenta

## ¿Puedo cambiar el propietario del posible cliente en Marketo? {#can-i-change-the-lead-owner-in-marketo}

Por supuesto, solo tiene que usar la acción de flujo [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}.

>[!NOTE]
>
>No puede cambiar la información del propietario con [Uso de la página de detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## ¿Qué puedo hacer con estos datos? {#what-can-i-do-with-this-data}

Existen muchas razones para utilizar estos datos, como

* Enviar un correo electrónico personalizado con la firma del propietario de ventas
* Filtre por representantes de ventas específicos para marketing o incluso para analizar la eficacia
* Reglas de asignación (y reasignación) en Marketo
* Úsalos en las acciones de flujo [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} y [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}

Marketo tiene una sincronización de [!DNL Salesforce] impresionante. ¡Nadie más lo hace tan bien!
