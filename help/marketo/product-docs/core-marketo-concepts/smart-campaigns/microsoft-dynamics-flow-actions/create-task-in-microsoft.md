---
unique-page-id: 37356429
description: Obtenga información sobre cómo crear una tarea en Microsoft Dynamics a partir de un paso de flujo. Cree una tarea para el propietario cuando alguien entre en el flujo.
title: Crear tarea en Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
TQID: https://experienceleague.adobe.com/qQL3O4Vi8ncdlXtk2gvraWzquz3oZx5B-1YWTkwdVac
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 4%

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
