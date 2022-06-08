---
unique-page-id: 7515131
description: Sincronización SFDC - Eliminación de un posible cliente/contacto - Documentos de Marketo - Documentación del producto
title: 'Sincronización SFDC: Eliminación de un posible cliente/contacto'
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Sincronización SFDC: Eliminación de un posible cliente o contacto {#sfdc-sync-deleting-a-lead-contact}

A continuación, algunos de los detalles:

* Marketo no elimina automáticamente a las personas solo porque los posibles clientes se eliminaron en Salesforce. En lugar de eso, el indicador de campo &quot;SFDC Is Deleted&quot; se establece en true. Si lo desea, puede crear un déclencheur de este campo para eliminarlo en Marketo.
* [Eliminar persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) acción de flujo. Esto elimina a una persona en MKTO, pero tiene la opción de eliminarla en `Salesforce` también.

* [Eliminar de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) acción de flujo: Esto elimina un posible cliente en SFDC, pero también tiene la opción de eliminar una persona en Marketo.
* Si se elimina un posible cliente en Salesforce (pero no se elimina a una persona en Marketo) y luego se ejecuta a través del [Sincronizar con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) acción de flujo, entonces crearía un nuevo posible cliente en Salesforce.
