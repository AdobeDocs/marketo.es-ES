---
unique-page-id: 7515131
description: Sincronización SFDC - Eliminación de un posible cliente/contacto - Documentos de Marketo - Documentación del producto
title: 'Sincronización SFDC: Eliminación de un posible cliente/contacto'
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Sincronización SFDC: Eliminación de un posible cliente/contacto {#sfdc-sync-deleting-a-lead-contact}

A continuación, algunos de los detalles:

* Marketo no elimina automáticamente a las personas solo porque los posibles clientes se eliminaron en Salesforce. En lugar de eso, el indicador de campo &quot;SFDC Is Deleted&quot; se establece en true. Si lo desea, puede crear un déclencheur de este campo para eliminarlo en Marketo.
* [Eliminar acción ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) de flujo de trabajo personal. Esto elimina a una persona en MKTO, pero también puede eliminar en `Salesforce`.

* [Eliminar de la acción ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow: Esto elimina un posible cliente en SFDC, pero también tiene la opción de eliminar una persona en Marketo.
* Si se elimina un posible cliente en Salesforce (pero no se elimina a una persona en Marketo) y luego se ejecuta a través de la acción de flujo [Sincronizar con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), entonces crearía un nuevo posible cliente en Salesforce.
