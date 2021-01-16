---
unique-page-id: 1147066
description: Anular restricciones de persona en una Campaña inteligente - Documentos de marketing - Documentación del producto
title: Anular restricciones de persona en una Campaña inteligente
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---


# Anular restricciones de persona en una Campaña inteligente {#override-person-restrictions-in-a-smart-campaign}

Marketo le permite establecer el número máximo de personas que pueden optar a una campaña inteligente; esto le ayuda a evitar enviar por correo electrónico accidentalmente toda la base de datos. Si desea _sobrescribir_ este límite, así es como.

>[!PREREQUISITES]
>
>Asegúrese de [habilitar las restricciones personales para campañas inteligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) en Administración de mercadotecnia.

1. En Actividades de marketing, vaya a la campaña inteligente y haga clic en **Programar**.

   ![](assets/one.png)

1. En Configuración de Campaña inteligente, haga clic en **Editar**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >El límite predeterminado es el establecido en Administración.

1. Escriba un nuevo límite y haga clic en **Guardar.**

   ![](assets/three.png)

   La campaña inteligente no se ejecutará si el número de personas que cumplen los requisitos supera el límite establecido.

   >[!CAUTION]
   >
   >Tenga cuidado con esta función para no incluir accidentalmente demasiadas personas.
