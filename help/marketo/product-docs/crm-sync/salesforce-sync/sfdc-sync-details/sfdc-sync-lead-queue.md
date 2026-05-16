---
unique-page-id: 7516241
description: Obtenga información acerca de la asignación de personas a colas de posibles clientes de Salesforce desde Marketo. Utilice las acciones Sincronizar persona con SFDC o Cambiar propietario para la distribución de posibles clientes.
title: 'Sincronización de SFDC: cola de posibles clientes'
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/aUrT7qSMy65t3K07O176nt-Bzjm9urgnXKAkZgs1-cs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 150
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
