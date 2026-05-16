---
unique-page-id: 1147066
description: Obtenga información sobre cómo anular las restricciones de persona en una campaña inteligente. Permitir que las personas se ejecuten incluso si alcanzan los límites de comunicación.
title: Anulación de restricciones de una persona en una campaña inteligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/GUIwrHBCrtl5NONZAqCY9sXt1FaLfjBwe3N3t1u98a4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 9%

---

# Anulación de restricciones de una persona en una campaña inteligente {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage le permite establecer el número máximo de personas que pueden optar a una campaña inteligente; esto le ayuda a evitar enviar por correo electrónico accidentalmente toda la base de datos. Si desea _anular_ este límite, así es como debe hacerlo.

>[!PREREQUISITES]
>
>Asegúrese de [habilitar restricciones de persona para campañas inteligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} en el administrador de Marketo.

1. En **[!UICONTROL Actividades de marketing]**, vaya a su campaña inteligente y haga clic en **[!UICONTROL Programar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. En Configuración de campañas inteligentes, haga clic en **[!UICONTROL Editar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >El límite predeterminado es el establecido en Administración.

1. Introduce un nuevo límite y haz clic en **[!UICONTROL Guardar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campaña inteligente no se ejecutará si el número de personas aptas supera el límite establecido.

   >[!CAUTION]
   >
   >Tenga cuidado con esta función para no incluir accidentalmente a demasiadas personas.
