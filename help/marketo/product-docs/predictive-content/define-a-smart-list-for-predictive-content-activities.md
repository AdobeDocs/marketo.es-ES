---
unique-page-id: 10097873
description: Definición de una lista inteligente para actividades de contenido predictivo - Documentos de Marketo - Documentación del producto
title: Definir una lista inteligente para actividades de contenido predictivo
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Definir una lista inteligente para actividades de contenido predictivo {#define-a-smart-list-for-predictive-content-activities}

Puede utilizar actividades de contenido predictivo en déclencheur y filtros al definir una lista inteligente en una campaña inteligente. Puede almacenar en déclencheur una acción para cualquiera que haga clic en contenido predictivo a través de [Rich Media template](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), [Content Recommendations Bar](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) o en un [correo electrónico](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. En su campaña inteligente, vaya a la ficha **[!UICONTROL Lista inteligente]**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Las listas inteligentes pueden hacer cosas increíbles. Obtenga más información en la [lista inteligente en profundidad](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Busque el déclencheur y, a continuación, arrástrelo y suéltelo en el lienzo.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Una campaña inteligente con déclencheur se ejecuta en modo de Déclencheur. Se ejecuta en una persona a la vez en función de los eventos activados y los filtros añadidos.

1. Haga clic en el menú desplegable **[!UICONTROL Nombre]** y seleccione un operador.

   ![](assets/smart-list-dropdown-hands.png)

1. Defina el déclencheur.

   ![](assets/smart-lislt-select-content-hands.png)

1. Agregar la restricción **[!UICONTROL Type]**.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Seleccione el origen que necesite para la lista inteligente.

   ![](assets/pc-add-constraint.png)

1. Si usas el origen del correo electrónico para el contenido predictivo, agrega el déclencheur **[!UICONTROL Clicks Link in Email]**. Seleccione su correo electrónico y agregue la restricción **[!UICONTROL Is Predictive]**, definida como **[!UICONTROL true]**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Añada otros filtros según sea necesario.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >En una campaña inteligente con déclencheur y filtros, los déclencheur aparecen en la parte superior. Cuando se activa, solo las personas que cumplen los criterios de filtro pasan por el flujo.

   >[!NOTE]
   >
   >Con varios déclencheur, una persona pasa al flujo si se activa CUALQUIERA de los déclencheur.

   Para ejecutar la campaña en un conjunto de personas al mismo tiempo, aprende a [definir una lista inteligente para una campaña inteligente por lotes](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definir lista inteligente para campaña inteligente | Lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Agregar un paso de flujo a una campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definir una lista inteligente para actividades de Web Personalization](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Habilitar contenido predictivo para medios enriquecidos en web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Habilitar la barra de recomendaciones de contenido](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)
