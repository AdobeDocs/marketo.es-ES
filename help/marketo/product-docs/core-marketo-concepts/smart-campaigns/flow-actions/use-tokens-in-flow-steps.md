---
unique-page-id: 1146995
description: 'Usar tokens en pasos de flujo: documentos de marketing: documentación del producto'
title: Usar tokens en pasos de flujo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Usar tokens en pasos de flujo {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>* [Añadir un paso de flujo en una Campaña inteligente](add-a-flow-step-to-a-smart-campaign.md)


Un token es una variable. Lo usas en [correos electrónicos](https://docs.marketo.com/pages/viewpage.action?pageId=557076), [páginas de aterrizaje](https://docs.marketo.com/pages/viewpage.action?pageId=2359689)y campañas [](https://docs.marketo.com/display/DOCS/Smart+Lists+and+Lists) inteligentes para facilitar tu vida. Puede utilizar [Mis tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (tokens personalizados) en pasos de flujo, enlaces web, correos electrónicos y páginas de aterrizaje.  Puede utilizar tokens para incluir contenido variable en estos pasos de flujo:

* Cambiar valor de datos
* Momento interesante
* Pasos de Campaña de Salesforce (agregar, quitar, cambiar estado)
* Crear Tarea
* Enviar alerta (solo en campañas desencadenadoras)

>[!NOTE]
>
>**Disponibilidad**
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

1. En el paso de flujo, escriba el inicio `{{` para obtener categorías de token. ![](assets/image2014-9-22-14-3a3-3a17.png)>

   >[!NOTE]
   >
   >**Buceo profundo**
   >
   >Consulte [Información general](../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) de tokens para obtener una lista de varios tokens disponibles.

1. Continúe escribiendo hasta que encuentre el token que desea y haga clic para seleccionarlo.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Se pueden utilizar varios tokens en los pasos de flujo de mensajes de aviso de Momento interesante, Crear Tarea y Enviar alerta.

   >[!NOTE]
   >
   >**Artículos relacionados**
   >
   >* [Administración de mis tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Explicación de mis tokens en un Programa](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)


¡Genial! Los datos se extraerán del token cuando se ejecute la campaña inteligente.