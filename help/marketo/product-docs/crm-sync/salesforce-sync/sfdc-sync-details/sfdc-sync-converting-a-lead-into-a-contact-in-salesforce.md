---
unique-page-id: 2953465
description: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce. Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce'
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine tres escenarios diferentes en Salesforce: (no usar [Paso Convertir flujo de persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} en Marketo Engage)

1. Conversión de un posible cliente en una **nuevo contacto y nueva cuenta**
1. Conversión de un posible cliente en una **nuevo contacto** en un **cuenta existente**

1. Conversión de un posible cliente en un **contacto existente** en un **cuenta existente** (funciona igual que [fusión](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

En los tres casos terminas con **1 contacto y ningún posible cliente en Salesforce y 1 contacto y ninguna persona en Marketo.**

En Marketo, el registro tendrá ahora un tipo de SFDC = Contacto.

>[!TIP]
>
>Al realizar la conversión en Salesforce, asegúrese de que [los campos personalizados de posible cliente están bien asignados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}. No desea perder ningún dato de.

Puede aplicar déclencheur y filtros mediante: &quot;El posible cliente se ha convertido&quot; y &quot;El posible cliente se ha convertido&quot;.
