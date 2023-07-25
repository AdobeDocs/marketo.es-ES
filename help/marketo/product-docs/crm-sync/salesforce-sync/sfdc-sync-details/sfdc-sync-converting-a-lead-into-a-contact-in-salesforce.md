---
unique-page-id: 2953465
description: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce. Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce'
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine tres escenarios diferentes en Salesforce: (no usar [Paso Convertir flujo de persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) en Marketo)

1. Conversión de un posible cliente en una **nuevo contacto y nueva cuenta**
1. Conversión de un posible cliente en una **nuevo contacto** en un **cuenta existente**

1. Conversión de un posible cliente en un **contacto existente** en un **cuenta existente** (funciona igual que [fusión](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

En los tres casos terminas con **1 contacto y ningún posible cliente en Salesforce y 1 contacto y ninguna persona en Marketo.**

En Marketo, el registro tendrá ahora un tipo de SFDC = Contacto.

>[!TIP]
>
>Al realizar la conversión en Salesforce, asegúrese de que [los campos personalizados de posible cliente están bien asignados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). No desea perder ningún dato de.

Puede aplicar déclencheur y filtros mediante: &quot;El posible cliente se ha convertido&quot; y &quot;El posible cliente se ha convertido&quot;.
