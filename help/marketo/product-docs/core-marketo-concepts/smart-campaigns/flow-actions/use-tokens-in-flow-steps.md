---
unique-page-id: 1146995
description: 'Uso de tokens en los pasos de flujo: Documentos de Marketo: Documentación del producto'
title: Uso de tokens en pasos de flujo
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Utilizar tokens en los pasos de flujo {#use-tokens-in-flow-steps}

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más información.

>[!PREREQUISITES]
>
>[Adición de un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Un token es una variable. Lo utiliza en correos electrónicos, páginas de aterrizaje y campañas inteligentes para facilitar las cosas. Puede utilizar [Mis tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (tokens personalizados) en pasos de flujo, enlaces web, correos electrónicos y páginas de aterrizaje. Puede utilizar tokens para incluir contenido variable en estos pasos de flujo:

* Cambiar valor de datos
* Cambiar datos de miembros del programa
* Momento interesante
* Pasos de la campaña de Salesforce (añadir, quitar, cambiar estado)
* Crear tarea
* Enviar alerta (solo en campañas de déclencheur)

1. En el paso de flujo, empiece a escribir `{{` para obtener categorías de token. ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Consulte [Información general de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) para obtener una lista de varios tokens disponibles.

1. Siga escribiendo hasta que encuentre el token que desee y haga clic en para seleccionarlo.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Se pueden utilizar varios tokens en los pasos de flujo Momento interesante, Crear tarea y Enviar alerta.

   >[!NOTE]
   >
   >Los tokens de campo personalizados de miembro del programa se pueden usar en: Crear tarea, Crear tarea en Microsoft, Momentos interesantes, Acciones de flujo de cambio de valor de datos y Webhooks.

   ¡Genial! Los datos se extraerán del token cuando se ejecute la campaña inteligente.

   >[!MORELIKETHIS]
   >
   >* [Administración de tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Explicación de mis tokens en un programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

