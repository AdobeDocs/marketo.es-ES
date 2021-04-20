---
title: override-person-constraint-in-a-smart-campaign
description: Anular restricciones de personas en una campaña inteligente
exl-id: efdd6c68-a95e-4b2a-9249-e2e1f550b628
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---

# Anular restricciones de personas en una campaña inteligente

<br> 

Marketo le permite establecer el número máximo de personas que pueden cumplir los requisitos para una campaña inteligente; esto le ayuda a evitar enviar por correo electrónico accidentalmente toda la base de datos. Si desea anular este límite, así es como.

>[!IMPORTANT]
>
>Asegúrese de [habilitar restricciones personales para campañas inteligentes](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) en Marketo [!UICONTROL Admin].

1. Busque la campaña inteligente y haga clic en **[!UICONTROL Schedule]**.

   ![Imagen uno](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Haga clic en **[!UICONTROL Reglas de clasificación]**.

   ![Imagen dos](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >El límite predeterminado es el establecido en Administración.

1. Junto a **[!UICONTROL Anular campaña si los posibles clientes cualificados exceden]**, introduzca un nuevo límite.

   ![Imagen tres](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>La campaña inteligente no se ejecutará si el número de personas que cumplen los requisitos supera el límite establecido.

>[!CAUTION]
>
>Tenga cuidado con esta función para no incluir accidentalmente demasiadas personas.
