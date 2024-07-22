---
unique-page-id: 7515131
description: 'Sincronización de SFDC: eliminación de un posible cliente/contacto - Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: eliminación de un posible cliente/contacto'
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Sincronización de SFDC: eliminación de un posible cliente/contacto {#sfdc-sync-deleting-a-lead-contact}

Estos son algunos de los detalles:

* Marketo Engage no elimina automáticamente personas solo porque se eliminaron posibles clientes en Salesforce. En lugar de ello, el indicador &quot;SFDC is Deleted&quot; se establece en true. Si lo desea, puede eliminar este campo del déclencheur para eliminarlo en Marketo.
* [Eliminar persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md){target="_blank"} acción de flujo. Esto elimina a una persona en MKTO, pero tiene la opción de eliminarla también en `Salesforce`.

* [Eliminar de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md){target="_blank"} acción de flujo: esto elimina un posible cliente de SFDC, pero tiene la opción de eliminar también a una persona de Marketo.
* Si se elimina un posible cliente en Salesforce (pero una persona no se elimina en Marketo) y luego se ejecuta a través de la acción de flujo [Sincronizar con Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}, se crearía un nuevo posible cliente en Salesforce.
