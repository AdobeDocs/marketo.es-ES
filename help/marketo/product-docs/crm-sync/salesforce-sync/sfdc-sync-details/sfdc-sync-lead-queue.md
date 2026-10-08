---
unique-page-id: 7516241
description: Obtenga información acerca de la asignación de personas a colas de posibles clientes de Salesforce desde Marketo. Utilice las acciones Sincronizar persona con SFDC o Cambiar propietario para la distribución de posibles clientes.
title: 'Sincronización de SFDC: cola de posibles clientes'
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/aUrT7qSMy65t3K07O176nt-Bzjm9urgnXKAkZgs1-cs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 17%
---
# Sincronización de SFDC: cola de posibles clientes {#sfdc-sync-lead-queue}

Marketo permite agregar personas a [[!DNL Salesforce] colas de posibles clientes](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) para ayudar con la distribución de posibles clientes. Aquí están los detalles.

## ¿Cómo asignar una persona a una cola en Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Puede asignar una persona a una cola de posibles clientes [!DNL Salesforce] mediante cualquiera de estas acciones de flujo:

* [Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Cambiar propietario](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>No puede crear ni cambiar colas en Marketo.

## ¿Cómo se almacena la información del propietario del posible cliente si la persona pertenece a una cola? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si un posible cliente es propiedad de una cola en [!DNL Salesforce], estos campos de propietario de ventas se mantienen vacíos hasta que se asigne el posible cliente a un propietario.

* Nombre del propietario de ventas
* Apellido del propietario de ventas
* Título de propietario de ventas
* Número de teléfono del propietario de ventas
* Dirección de correo electrónico del propietario de ventas
