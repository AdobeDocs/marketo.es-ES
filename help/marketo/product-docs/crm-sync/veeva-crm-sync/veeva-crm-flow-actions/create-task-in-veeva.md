---
description: Aprenda a crear tareas en Veeva desde Marketo para informar a las ventas qué hacer y cuándo. Utilice el paso de flujo Crear tarea y personalice el asunto, la descripción y la fecha de vencimiento.
title: Crear tarea en  [!DNL Veeva]
exl-id: 342e45dd-2038-432d-a6b6-1740c8f0b58e
feature: Veeva CRM
TQID: https://experienceleague.adobe.com/W4zIWswN64cHyqA7oQ9iku0iMC7Q6NqIpWiAcSgvD04
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 0%

---

# Crear tarea en [!DNL Veeva] {#create-task-in-veeva}

Como experto en marketing, dispone de información que puede ayudar a las ventas a cerrar acuerdos. Puede crear tareas para que sepan lo que deben hacer y cuándo deben hacerlo.

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>Cuando el usuario de sincronización de Marketo está creando tareas, **[!UICONTROL Vence en]** es un campo obligatorio para crear la tarea en [!DNL Veeva]. Marketo introducirá cinco días de forma predeterminada si no hay ningún valor.

De forma predeterminada, el paso de flujo tendrá este aspecto:

![](assets/create-task-in-veeva-2.png)

Personalice todos los campos para crear la tarea de la manera que desee.

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>Puede usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` y `{{system.tokens}}` en el [!UICONTROL Asunto] y [!UICONTROL Descripción]. Consulte [Tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obtener más información.
