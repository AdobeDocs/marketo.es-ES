---
unique-page-id: 37356429
description: Crear tarea en Microsoft - Documentos de Marketo - Documentación del producto
title: Crear tarea en Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Crear tarea en Microsoft {#create-task-in-microsoft}

Como experto en marketing, dispone de información que puede ayudar a las ventas a cerrar acuerdos. Puede crear tareas para que sepan lo que deben hacer y cuándo deben hacerlo.

Crear tarea en Microsoft crea una tarea en Actividades relacionadas con la persona (posible cliente o contacto) en [!DNL Microsoft].

>[!NOTE]
>
>Este paso de flujo _solo funciona cuando se utiliza con déclencheur_, no filtros, en su campaña inteligente.

De forma predeterminada, el paso de flujo tendrá este aspecto:

![](assets/msd1.png)

>[!NOTE]
>
>Cuando el usuario de sincronización de Marketo está creando tareas, **[!UICONTROL Vence en]** es un campo obligatorio para crear la tarea en [!DNL Microsoft]. Marketo introducirá cinco días de forma predeterminada si no se introduce ningún valor.

Personalice todos los campos para crear la tarea de la manera que desee.

![](assets/msd2.png)

>[!NOTE]
>
>El campo &quot;Estado&quot; especificado para la tarea en Acción de flujo actualiza el campo: &quot;Razón del estado&quot; en [!DNL Microsoft].

>[!TIP]
>
>Puede utilizar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` y `{{system.tokens}}` en el **[!UICONTROL Asunto]** y **[!UICONTROL Descripción]**. Consulte [Tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obtener más información.
