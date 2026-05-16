---
unique-page-id: 7515131
description: Comprender cómo funciona la eliminación de contactos y posibles clientes entre Salesforce y Marketo. Obtenga información sobre las acciones de flujo de SFDC Eliminar persona y Eliminar de SFDC.
title: 'Sincronización de SFDC: eliminación de un posible cliente/contacto'
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/v0nRloqmlp-iedcmE4DdATxpYXnvB13cxkEn7809Hy4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 4%

---

# Sincronización de SFDC: eliminación de un posible cliente/contacto {#sfdc-sync-deleting-a-lead-contact}

Estos son algunos de los detalles:

* Marketo no elimina a las personas automáticamente solo porque se eliminaron posibles clientes en [!DNL Salesforce]. En lugar de ello, el indicador &quot;SFDC is Deleted&quot; se establece en true. Si lo desea, puede eliminar este campo del déclencheur para eliminarlo en Marketo.
* [Eliminar persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) acción de flujo. Esto elimina a una persona en MKTO, pero tiene la opción de eliminarla también en `Salesforce`.

* [Eliminar de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) acción de flujo: Esto elimina un posible cliente en SFDC, pero tiene la opción de eliminar también a una persona en Marketo.
* Si se elimina un posible cliente en [!DNL Salesforce] (pero una persona no se elimina en Marketo) y posteriormente se ejecuta la acción de flujo [Sincronizar con [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), se crearía un nuevo posible cliente en [!DNL Salesforce].
