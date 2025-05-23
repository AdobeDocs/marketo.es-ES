---
unique-page-id: 7516241
description: 'Sincronización de SFDC: cola de posibles clientes, documentos de Marketo, documentación del producto'
title: 'Sincronización de SFDC: cola de posibles clientes'
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 11%

---

# Sincronización de SFDC: cola de posibles clientes {#sfdc-sync-lead-queue}

El Marketo Engage le permite agregar personas a [colas de posibles clientes de Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm){target="_blank"} para ayudar con la distribución de posibles clientes. Aquí están los detalles.

## ¿Cómo asignar una persona a una cola en Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Puede asignar una persona a una cola de posibles clientes de Salesforce mediante cualquiera de estas acciones de flujo:

* [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>No puede crear ni cambiar colas en Marketo.

## ¿Cómo se almacena la información del propietario del posible cliente si la persona pertenece a una cola? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si un posible cliente es propiedad de una cola en Salesforce, estos campos de propietario de ventas se mantienen vacíos hasta que el posible cliente se asigne a un propietario.

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título de propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de correo electrónico del propietario de ventas
