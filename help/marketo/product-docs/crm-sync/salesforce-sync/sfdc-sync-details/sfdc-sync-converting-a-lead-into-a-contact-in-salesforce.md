---
unique-page-id: 2953465
description: Sincronización de SFDC - Conversión de un posible cliente en un contacto en Salesforce - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce'
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Sincronización SFDC: Conversión de un posible cliente en un contacto en Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine tres escenarios diferentes en Salesforce: (no se utiliza el [paso de flujo de Convertir persona](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) en Marketing)

1. Conversión de un posible cliente en un **nuevo contacto y nueva cuenta**
1. Conversión de un posible cliente en un **nuevo contacto** en una **cuenta existente**

1. Conversión de un posible cliente en un **contacto existente** en una **cuenta existente** (funciona igual que [combinación](sfdc-sync-merging-a-lead-contact-person.md))

En los tres casos, usted termina con **1 contacto y ningún posible cliente en Salesforce y 1 contacto y ninguna persona en Marketing.**

En Marketing, el registro ahora tendrá un tipo SFDC = Contacto.

>[!TIP]
>
>Al realizar la conversión en Salesforce, asegúrese de que los campos personalizados de [posibles clientes están correctamente asignados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). No desea perder ningún dato.

Puede activar y filtrar mediante: &quot;El posible cliente es convertido&quot; y &quot;El posible cliente fue convertido&quot;.