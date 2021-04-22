---
unique-page-id: 37356429
description: Crear tarea en Microsoft - Marketo Docs - Documentación del producto
title: Crear tarea en Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Crear tarea en Microsoft {#create-task-in-microsoft}

Como especialista en marketing, tiene información que puede ayudar a las ventas a cerrar ofertas. Puede crear tareas para que sepan qué deben hacer y cuándo deben hacerlo.

Crear tarea en Microsoft crea una tarea en Actividades relacionadas con la persona (posible cliente o contacto) en Microsoft.

>[!NOTE]
>
>Este paso de flujo **solo funcionará cuando se utilice con déclencheur**, no con filtros, en la campaña inteligente.

De forma predeterminada, el paso de flujo tendrá este aspecto:

![](assets/msd1.png)

>[!NOTE]
>
>Cuando el usuario de sincronización de Marketo está creando tareas, **Due In** es un campo obligatorio para la tarea que se creará en Microsoft. Marketo introducirá cinco días de forma predeterminada si no se introduce ningún valor.

Personalice todos los campos para crear la tarea del modo que desee.

![](assets/msd2.png)

>[!NOTE]
>
>El campo &quot;Estado&quot; especificado para la tarea en Acción de flujo actualiza el campo: &quot;Motivo del estado&quot; en Microsoft.

>[!TIP]
>
>Puede utilizar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` y `{{system.tokens}}` en **Subject** y **Description**. Consulte [Tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) para obtener más información.
