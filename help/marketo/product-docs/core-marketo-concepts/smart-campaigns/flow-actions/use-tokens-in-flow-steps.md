---
unique-page-id: 1146995
description: 'Uso de tokens en pasos de flujo: documentos de Marketo, documentación del producto'
title: Uso de tokens en pasos de flujo
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 5%

---

# Uso de tokens en pasos de flujo {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Un token es una variable. Lo utiliza en correos electrónicos, páginas de aterrizaje y campañas inteligentes para facilitarle la vida. Puede utilizar [Mis tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (tokens personalizados) en pasos de flujo, webhooks, correos electrónicos y páginas de aterrizaje. Puede utilizar tokens para incluir contenido variable en estos pasos del flujo:

* Cambiar valor de datos
* Cambiar datos del miembro del programa
* Momento interesante
* Pasos de la campaña de Salesforce (añadir, eliminar, cambiar el estado)
* Crear tarea
* Enviar alerta (solo en campañas de Déclencheur)

1. En el paso de flujo, empiece a escribir `{{` para obtener las categorías de token.

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Desproteger [Información general sobre tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} para obtener una lista de varios tokens disponibles.

1. Siga escribiendo hasta que encuentre el token que desee y haga clic en para seleccionar.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Se pueden utilizar varios tokens en los pasos de flujo Momento interesante, Crear tarea y Enviar alerta.

   >[!NOTE]
   >
   >Los tokens de campo personalizado de miembro de programa se pueden utilizar en: Crear tarea, Crear tarea en Microsoft, Momentos interesantes, Cambiar valor de datos, Acciones de flujo y Webhooks.

   ¡Genial! Los datos se extraerán del token cuando se ejecute la campaña inteligente.

   >[!MORELIKETHIS]
   >
   >* [Administrar mis tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Explicación de mis tokens en un programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
