---
unique-page-id: 1147066
description: 'Anulación de restricciones de persona en una campaña inteligente: documentos de Marketo, documentación del producto'
title: Anulación de restricciones de persona en una campaña inteligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: fec5219c599c805328d77797d2636e549e489ca5
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Anulación de restricciones de persona en una campaña inteligente {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage le permite establecer el número máximo de personas que pueden cumplir los requisitos para una campaña inteligente; esto le ayuda a evitar enviar por correo electrónico accidentalmente toda la base de datos. Si lo desea _invalidar_ este límite, así es como.

>[!PREREQUISITES]
>
>Asegúrese de [habilitar restricciones de persona para campañas inteligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} en Administración de Marketo.

1. En Actividades de marketing, vaya a la campaña inteligente y haga clic en **Programación**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. En Configuración de campaña inteligente, haga clic en **[!UICONTROL Editar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >El límite predeterminado es el establecido en Administración.

1. Introduzca un nuevo límite y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campaña inteligente no se ejecutará si el número de personas aptas supera el límite establecido.

   >[!CAUTION]
   >
   >Tenga cuidado con esta función para no incluir accidentalmente a demasiadas personas.
