---
unique-page-id: 7516241
description: Sincronización SFDC - Cola de posibles clientes - Documentos de Marketo - Documentación del producto
title: Sincronización de SFDC - Cola de posibles clientes
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 15%

---

# Sincronización SFDC: Cola de posibles clientes {#sfdc-sync-lead-queue}

Marketo le permite agregar personas a [Colas de posibles clientes de Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) para ayudar con la distribución de posibles clientes. Aquí están los detalles.

## ¿Cómo asignar una persona a una cola en Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Puede asignar una persona a una cola de posibles clientes de Salesforce mediante cualquiera de estas acciones de flujo:

* [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>No se pueden crear ni cambiar colas en Marketo.

## ¿Cómo se almacena la información del propietario del posible cliente si la persona pertenece a una cola? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si un posible cliente es propiedad de una cola de Salesforce, estos campos de propietario de ventas se mantienen vacíos hasta que el posible cliente se asigna a un propietario.

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título del propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de email del propietario de ventas
