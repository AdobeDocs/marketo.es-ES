---
unique-page-id: 37356429
description: Crear tarea en Microsoft - Documentos de Marketo - Documentación del producto
title: Crear tarea en Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Crear tarea en Microsoft {#create-task-in-microsoft}

Como experto en marketing, dispone de información que puede ayudar a las ventas a cerrar acuerdos. Puede crear tareas para que sepan lo que deben hacer y cuándo deben hacerlo.

Crear tarea en Microsoft crea una tarea en Actividades relacionadas con la persona (posible cliente o contacto) en [!DNL Microsoft].

>[!NOTE]
>
>Este paso de flujo _solo funcionará cuando se use con déclencheur_, no con filtros, en su campaña inteligente.

De forma predeterminada, el paso de flujo tendrá este aspecto:

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Cuando el usuario de sincronización de Marketo está creando tareas, **[!UICONTROL Vence en]** es un campo obligatorio para crear la tarea en [!DNL Microsoft]. Marketo introducirá cinco días de forma predeterminada si no se introduce ningún valor.

Personalice todos los campos para crear la tarea de la manera que desee.

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>El campo &quot;Estado&quot; especificado para la tarea en Acción de flujo actualiza el campo: &quot;Motivo del estado&quot; en [!DNL Microsoft].

>[!TIP]
>
>Puede usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` y `{{system.tokens}}` en el **[!UICONTROL Asunto]** y **[!UICONTROL Descripción]**. Consulte [Tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obtener más información.
