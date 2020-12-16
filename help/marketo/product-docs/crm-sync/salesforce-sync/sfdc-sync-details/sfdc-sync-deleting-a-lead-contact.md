---
unique-page-id: 7515131
description: Sincronización de SFDC - Eliminación de un posible cliente/contacto - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: eliminación de un posible cliente o contacto'
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Sincronización SFDC: Eliminación de un posible cliente o contacto {#sfdc-sync-deleting-a-lead-contact}

Aquí están algunos de los detalles:

* Marketing no elimina automáticamente a las personas solo porque se eliminaron los leads en Salesforce. En su lugar, el indicador &quot;SFDC se elimina&quot; se establece en true. Si lo desea, puede activar este campo para eliminarlo de Marketing.
* [Acción Eliminar flujo de persona](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) . Esto elimina a una persona en MKTO, pero usted también tiene la opción de eliminar en `Salesforce` .

* [Acción Eliminar de flujo SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) : Esto elimina un posible cliente en SFDC, pero también tiene la opción de eliminar a una persona en Marketing Cloud.
* Si se elimina un posible cliente en Salesforce (pero no se elimina a una persona en Marketing) y luego se ejecuta mediante la acción de flujo [Sincronizar con Salesforce](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) , se crearía un nuevo posible cliente en Salesforce.

En otras palabras, ¡funciona como la magia!

![--](assets/image2015-5-20-15-3a3-3a27.png)

