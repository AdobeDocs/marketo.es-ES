---
title: override-personalmente-restrictions-in-a-smart-campaña
description: Anular restricciones de persona en una Campaña inteligente
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Anular restricciones de persona en una Campaña inteligente

<br> 

Marketo le permite establecer el número máximo de personas que pueden optar a una campaña inteligente; esto le ayuda a evitar enviar por correo electrónico accidentalmente toda la base de datos. Si quieres anular este límite, así es como.

>[!IMPORTANT]
>
>Asegúrese de [habilitar las restricciones personales para campañas inteligentes](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) en Marketing [!UICONTROL Administración].

1. Busque su campaña inteligente y haga clic en **[!UICONTROL Programar]**.

   ![Imagen uno](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Haga clic en **[!UICONTROL Reglas de clasificación]**.

   ![Imagen dos](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >El límite predeterminado es el establecido en Administración.

1. Junto a **[!UICONTROL Anular campaña si los leads cualificados exceden]**, introduzca un nuevo límite.

   ![Imagen tres](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>La campaña inteligente no se ejecutará si el número de personas que cumplen los requisitos supera el límite establecido.

>[!CAUTION]
>
>Tenga cuidado con esta función para no incluir demasiadas personas accidentalmente.
