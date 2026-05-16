---
unique-page-id: 1147017
description: Aprenda a crear una tarea de Salesforce en un paso de flujo. Cree una tarea para el propietario del posible cliente cuando alguien entre en el flujo.
title: Crear tarea
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/RJ5nZrVvURtgXEWWZwL2xXzlYOhWjKGSbX-MFTWCwzg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 130
ht-degree: 3%

---

# Crear tarea {#create-task}

Como experto en marketing, dispone de información que puede ayudar a las ventas a cerrar acuerdos. Puede crear tareas para que sepan lo que deben hacer y cuándo deben hacerlo.

![](assets/create-task-1.png)

>[!NOTE]
>
>Cuando el usuario de sincronización de Marketo está creando tareas, **[!UICONTROL Vence en]** es un campo obligatorio para que la tarea se cree en Salesforce. Marketo introducirá cinco días de forma predeterminada si no hay ningún valor.

De forma predeterminada, el paso de flujo tendrá este aspecto:

![](assets/create-task-2.png)

Personalice todos los campos para crear la tarea de la manera que desee.

![](assets/create-task-3.png)

>[!TIP]
>
>Puede usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` y `{{system.tokens}}` en el **[!UICONTROL Asunto]** y **[!UICONTROL Descripción]**. Consulte [Tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obtener más información.
