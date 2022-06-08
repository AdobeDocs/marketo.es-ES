---
unique-page-id: 2953465
description: 'Sincronización SFDC: conversión de un posible cliente en un contacto en Salesforce, Marketo Docs, documentación del producto'
title: 'Sincronización SFDC: conversión de un posible cliente en un contacto en Salesforce'
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincronización SFDC: Conversión de un posible cliente en un contacto en Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine tres escenarios diferentes en Salesforce: (sin usar la variable [Paso Convertir flujo de persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) en Marketo)

1. Conversión de un posible cliente en un **nuevo contacto y nueva cuenta**
1. Conversión de un posible cliente en un **nuevo contacto** en un **cuenta existente**

1. Conversión de un posible cliente en un **contacto existente** en un **cuenta existente** (funciona de forma idéntica a [combinación](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

En los tres casos terminas con **1 contacto y ningún posible cliente en Salesforce y 1 contacto y ninguna persona en Marketo.**

En Marketo, el registro ahora tendrá un Tipo de SFDC = Contacto.

>[!TIP]
>
>Al convertir en Salesforce, asegúrese de que su [Los campos personalizados de posibles clientes están bien asignados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). No desea perder ningún dato.

Puede filtrar y filtrar mediante: &quot;El posible cliente es convertido&quot; y &quot;El posible cliente fue convertido&quot;.
