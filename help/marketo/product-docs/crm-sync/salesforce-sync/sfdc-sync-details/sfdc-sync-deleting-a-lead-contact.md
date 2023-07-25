---
unique-page-id: 7515131
description: 'Sincronización de SFDC: eliminación de un posible cliente/contacto - Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: eliminación de un posible cliente/contacto'
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Sincronización de SFDC: eliminación de un posible cliente/contacto {#sfdc-sync-deleting-a-lead-contact}

Estos son algunos de los detalles:

* Marketo no elimina automáticamente personas solo porque se eliminaron posibles clientes en Salesforce. En lugar de ello, el indicador &quot;SFDC is Deleted&quot; se establece en true. Si lo desea, puede eliminar este campo del déclencheur para eliminarlo en Marketo.
* [Eliminar persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) acción de flujo. Esto elimina a una persona en MKTO, pero tiene la opción de eliminarla en `Salesforce` también.

* [Eliminar de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) acción de flujo: Esto elimina un posible cliente en SFDC, pero tiene la opción de eliminar también a una persona en Marketo.
* Si se elimina un posible cliente en Salesforce (pero una persona no se elimina en Marketo) y luego se ejecuta a través del [Sincronizar con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) acción de flujo, entonces crearía un nuevo posible cliente en Salesforce.
