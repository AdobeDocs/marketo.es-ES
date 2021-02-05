---
unique-page-id: 10097873
description: Definir una Lista inteligente para Actividades de contenido predictivo - Documentos de marketing - Documentación del producto
title: Definir una Lista inteligente para Actividades de contenido predictivo
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# Definir una Lista inteligente para Actividades de contenido predictivo {#define-a-smart-list-for-predictive-content-activities}

>[!NOTE]
>
>Según la fecha de compra, la suscripción de marketing puede incluir Contenido predictivo de marketing o Contenido`<sup>AI</sup>`. Para aquellos que utilizan contenido predictivo, Marketing está activando las funciones de análisis de contenido`<sup>AI</sup>` hasta el 30 de abril de 2018. Para mantener estas funciones más allá de esa fecha, póngase en contacto con el administrador de éxito del cliente de Marketing to para actualizar a Contenido de marketing`<sup>AI</sup>`.

Puede utilizar actividades de contenido predictivo en déclencheur y filtros cuando defina una lista inteligente en una campaña inteligente. Puede déclencheur de una acción para cualquiera que haga clic en contenido predictivo mediante la [plantilla de medios enriquecidos](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), la [barra de recomendaciones de contenido](enabling-predictive-content/enable-the-content-recommendation-bar.md) o en un mensaje de correo electrónico.

1. En la campaña inteligente, navegue a la ficha **Lista inteligente**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >**Buceo profundo**
   >
   >
   >Las listas inteligentes pueden hacer cosas increíbles. Obtenga más información en el [buceo profundo de lista inteligente](../../product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Busque el déclencheur y arrástrelo y suéltelo en el lienzo.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Una campaña inteligente con déclencheur se ejecuta en modo Déclencheur. Funciona de una persona a la vez en función de los eventos activados y los filtros agregados.

1. Haga clic en la lista desplegable **Nombre** y seleccione un operador.

   ![](assets/smart-list-dropdown-hands.png)

1. Defina el déclencheur.

   ![](assets/smart-lislt-select-content-hands.png)

1. Añada la restricción **Type**.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Seleccione el origen que necesita para la lista inteligente.

   ![](assets/pc-add-constraint.png)

1. Si está utilizando el origen de correo electrónico para el contenido predictivo, agregue el déclencheur **Clicks Link en Correo electrónico **Clicks. Seleccione el correo electrónico y agregue la restricción **Es predictivo**, definida como **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Añada cualquier otro filtros según sea necesario.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >En una campaña inteligente con déclencheur y filtros, los déclencheur van en la parte superior. Cuando se activa, solo las personas que cumplen los criterios del filtro atraviesan el flujo.

   >[!NOTE]
   >
   >Con múltiples déclencheur, una persona pasa al flujo si ALGUNO de los déclencheur se activa.

   [definir una lista inteligente para una campaña inteligente por lotes](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [Definir Lista inteligente para Campaña inteligente | Lote](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >    * [Añadir un paso de flujo en una Campaña inteligente](../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >    * [Definir una Lista inteligente para Actividades de personalización web](../../product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >    * [Habilitar contenido predictivo para medios enriquecidos por Web](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >    * [Habilitar la barra de recomendaciones de contenido](enabling-predictive-content/enable-the-content-recommendation-bar.md)


Para ejecutar la campaña en un grupo de personas al mismo tiempo, aprenda a .