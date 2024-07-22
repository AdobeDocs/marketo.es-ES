---
unique-page-id: 1147066
description: 'Anulación de restricciones de persona en una campaña inteligente: documentos de Marketo, documentación del producto'
title: Anulación de restricciones de persona en una campaña inteligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Anulación de restricciones de persona en una campaña inteligente {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage le permite establecer el número máximo de personas que pueden cumplir los requisitos para una campaña inteligente; esto le ayuda a evitar enviar por correo electrónico accidentalmente toda la base de datos. Si desea _anular_ este límite, así es como debe hacerlo.

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
