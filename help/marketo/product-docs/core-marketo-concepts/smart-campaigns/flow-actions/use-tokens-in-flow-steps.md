---
unique-page-id: 1146995
description: Aprenda a utilizar tokens en los pasos de flujo. Inserte valores dinámicos en el contenido y los correos electrónicos de los pasos de flujo.
title: Uso de tókenes en pasos de flujo
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/0b1iseuF-rKtBcS2qPRdwnPPRYJxUNG9hzlJQxNJQdI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 10%

---

# Uso de tókenes en pasos de flujo {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Agregar un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Un token es una variable. Lo utiliza en correos electrónicos, páginas de aterrizaje y campañas inteligentes para facilitarle la vida. Puede usar [Mis tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (tokens personalizados) en pasos de flujo, enlaces web, correos electrónicos y páginas de aterrizaje. Puede utilizar tokens para incluir contenido variable en estos pasos del flujo:

* Cambiar valor de datos
* Cambiar datos del miembro del programa
* Momento interesante
* [!DNL Salesforce] pasos de campaña (agregar, quitar, cambiar estado)
* Crear tarea
* Enviar alerta (solo en campañas de Déclencheur)

1. En el paso de flujo, empiece a escribir `{{` para obtener las categorías de tokens.

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >Consulte [Información general de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} para obtener una lista de varios tokens disponibles.

1. Siga escribiendo hasta que encuentre el token que desee y haga clic en para seleccionar.

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >Se pueden utilizar varios tokens en los pasos de flujo Momento interesante, Crear tarea y Enviar alerta.

   >[!NOTE]
   >
   >Los tokens de campo personalizado de miembro de programa se pueden utilizar en: Crear tarea, Crear tarea en Microsoft, Momentos interesantes, Cambiar valor de datos, Acciones de flujo y Webhooks.

   Los datos se extraerán del token cuando se ejecute la campaña inteligente.

   >[!MORELIKETHIS]
   >
   >* [Administrar mis tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Explicación de mis tokens en un programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
