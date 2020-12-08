---
unique-page-id: 7516241
description: Sincronización de SFDC - Cola de posibles clientes - Documentos de marketing - Documentación del producto
title: 'Sincronización SFDC: Cola de posibles clientes'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Sincronización SFDC: Cola de posibles clientes {#sfdc-sync-lead-queue}

Marketing permite agregar personas a las colas [de posibles clientes de](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) Salesforce para ayudar en la distribución de posibles clientes. Aquí están los detalles.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## ¿Cómo asignar una persona a una cola de Marketing? {#how-to-assign-a-person-to-a-queue-in-marketo}

Puede asignar una persona a una cola de posibles clientes de Salesforce mediante cualquiera de estas acciones de flujo:

* [Sincronizar persona con SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Cambiar propietario](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>No puede crear ni cambiar colas en Marketing.

## ¿Cómo se almacena la información del propietario del posible cliente si la persona pertenece a una cola? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si un posible cliente es propiedad de una cola de Salesforce, estos campos de propietario de ventas se mantienen vacíos hasta que el posible cliente se asigna a un propietario.

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título del propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de correo electrónico del propietario de ventas

