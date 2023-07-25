---
unique-page-id: 1147017
description: 'Crear tarea: documentos de Marketo, documentación del producto'
title: Crear tarea
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Crear tarea {#create-task}

Como experto en marketing, dispone de información que puede ayudar a las ventas a cerrar acuerdos. Puede crear tareas para que sepan lo que deben hacer y cuándo deben hacerlo.

![](assets/image2014-9-22-14-3a54-3a46.png)

>[!NOTE]
>
>Cuando el usuario de sincronización de Marketo está creando tareas, **Vence en** es un campo obligatorio para la tarea que se va a crear en Salesforce. Marketo introducirá cinco días de forma predeterminada si no hay ningún valor.

De forma predeterminada, el paso de flujo tendrá este aspecto:

![](assets/image2014-9-22-14-3a54-3a49.png)

Personalice todos los campos para crear la tarea de la manera que desee.

![](assets/image2014-9-22-14-3a54-3a52.png)

>[!TIP]
>
>Puede utilizar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` y `{{system.tokens}}` en el **Asunto** y **Descripción**. Consulte [Tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) para obtener más información.
