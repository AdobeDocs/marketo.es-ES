---
unique-page-id: 2360243
description: Establezca un número máximo de personas que puedan cumplir los requisitos para una campaña inteligente para evitar enviar por correo electrónico accidentalmente toda la base de datos.
title: Habilitar restricciones de persona para campañas inteligentes
exl-id: 45bdaf3f-874c-493f-9746-440f7703713c
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/6VwkOwN9nTqSyNcXvzyggPTk0Um5x1GPXIp2DBf2kww'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 11%
---
# Habilitar restricciones de persona para campañas inteligentes {#enable-person-restrictions-for-smart-campaigns}

Hay una función en Marketo para limitar el _número máximo_ de personas que pueden calificar para una campaña inteligente. Esto evita enviar por correo electrónico toda la base de datos.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!CAUTION]
>
>Esto solo se aplica a campañas por lotes y programas de correo electrónico.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-1.png)

1. Haga clic en **[!UICONTROL Campaña inteligente]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-2.png)

1. Haga clic en **[!UICONTROL Editar]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-3.png)

   >[!CAUTION]
   >
   >Si el número de personas que cumplen los requisitos para ejecutar una campaña inteligente supera el límite establecido, no se ejecutará en absoluto.

1. Introduce un límite y haz clic en **[!UICONTROL Guardar]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-4.png)

   >[!TIP]
   >
   >Deshabilite esta función dejando este campo en blanco.

   >[!CAUTION]
   >
   >Este límite se aplica a todas las campañas inteligentes, pero se puede anular en el nivel de campaña. Aprenda a [anular las restricciones de persona en una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md).

>[!MORELIKETHIS]
>
>[Anular restricciones de persona en una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)
