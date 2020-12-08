---
unique-page-id: 2953465
description: Sincronización de SFDC - Conversión de un posible cliente en un contacto en Salesforce - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Sincronización SFDC: Conversión de un posible cliente en un contacto en Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Imagine tres escenarios diferentes en Salesforce: (no se utiliza el paso [Convertir persona en](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) Marketing)

1. Conversión de un posible cliente en un **nuevo contacto y una nueva cuenta**
1. Conversión de un posible cliente en un **nuevo contacto** en una cuenta **existente**

1. Conversión de un posible cliente en un contacto **** existente en una cuenta **** existente (funciona igual que la [combinación](sfdc-sync-merging-a-lead-contact-person.md))

En los tres casos terminas con **1 contacto y sin posibles clientes en Salesforce y 1 contacto y ninguna persona en Marketing.**

En Marketing, el registro ahora tendrá un tipo SFDC = Contacto.

>[!TIP]
>
>Al realizar la conversión en Salesforce, asegúrese de que los campos personalizados de [posibles clientes están bien](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)asignados. No desea perder ningún dato.

Puede activar y filtrar mediante: &quot;El posible cliente es convertido&quot; y &quot;El posible cliente fue convertido&quot;.