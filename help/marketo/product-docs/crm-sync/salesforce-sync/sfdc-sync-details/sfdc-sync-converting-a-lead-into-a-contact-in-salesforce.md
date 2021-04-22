---
unique-page-id: 2953465
description: 'Sincronización SFDC: conversión de un posible cliente en un contacto en Salesforce, Marketo Docs, documentación del producto'
title: 'Sincronización SFDC: conversión de un posible cliente en un contacto en Salesforce'
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincronización SFDC: Conversión de un posible cliente en un contacto en Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine tres escenarios diferentes en Salesforce: (no se utiliza el paso [Convertir flujo de persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) en Marketo)

1. Conversión de un posible cliente en un **nuevo contacto y nueva cuenta**
1. Conversión de un posible cliente en un **nuevo contacto** en una **cuenta existente**

1. Conversión de un posible cliente en un **contacto existente** en una **cuenta existente** (esto funciona igual a [fusión](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

En los tres casos, usted termina con **1 contacto y no hay posibles clientes en Salesforce y 1 contacto y ninguna persona en Marketo.**

En Marketo, el registro ahora tendrá un Tipo de SFDC = Contacto.

>[!TIP]
>
>Al convertir en Salesforce, asegúrese de que los campos personalizados de [posibles clientes estén correctamente asignados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). No desea perder ningún dato.

Puede filtrar y filtrar mediante: &quot;El posible cliente es convertido&quot; y &quot;El posible cliente fue convertido&quot;.
