---
unique-page-id: 2953465
description: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce. Documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: conversión de un posible cliente en un contacto en Salesforce'
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Sincronización de SFDC: convertir un posible cliente en un contacto en [!DNL Salesforce] {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine tres escenarios diferentes en [!DNL Salesforce]: (sin usar el paso [Convertir flujo de persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) en Marketo)

1. Convirtiendo un posible cliente en **nuevo contacto y nueva cuenta**
1. Convirtiendo un posible cliente en **nuevo contacto** en una **cuenta existente**

1. Convirtiendo un posible cliente en un **contacto existente** en una **cuenta existente** (esto funciona igual que [combinar](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

En los tres casos, terminas con **1 contacto y sin posibles clientes en [!DNL Salesforce] y 1 contacto y sin personas en Marketo.**

En Marketo, el registro tendrá ahora un tipo de SFDC = Contacto.

>[!TIP]
>
>Al convertir en [!DNL Salesforce], asegúrese de que los [campos personalizados de posible cliente estén bien asignados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). No desea perder ningún dato de.

Puede filtrar y almacenar en déclencheur mediante: &quot;[!UICONTROL El posible cliente se ha convertido]&quot; y &quot;[!UICONTROL El posible cliente se ha convertido]&quot;.&quot;
