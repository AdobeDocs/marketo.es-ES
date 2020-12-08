---
unique-page-id: 10097873
description: Definir una Lista inteligente para Actividades de contenido predictivo - Documentos de marketing - Documentación del producto
title: Definir una Lista inteligente para Actividades de contenido predictivo
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# Definir una Lista inteligente para Actividades de contenido predictivo {#define-a-smart-list-for-predictive-content-activities}

>[!NOTE]
>
>Según la fecha de compra, la suscripción de marketing puede incluir Contenido`<sup>AI</sup>`predictivo de marketing o Contenido. Para aquellos que utilizan contenido predictivo, Marketing`<sup>AI</sup>` está activando las funciones de Content Analytics hasta el 30 de abril de 2018. Para mantener estas funciones más allá de esa fecha, póngase en contacto con el administrador de éxito del cliente de Marketing to para actualizar a Contenido`<sup>AI</sup>`de marketing.

Puede utilizar actividades de contenido predictivo en activadores y filtros cuando defina una lista inteligente en una campaña inteligente. Puede activar una acción para cualquiera que haga clic en contenido predictivo a través de la plantilla [de medios](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)enriquecidos, la barra [de recomendaciones de](enabling-predictive-content/enable-the-content-recommendation-bar.md)contenido o un mensaje de correo electrónico.

1. En la campaña inteligente, vaya a la ficha Lista **** inteligente.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >**Buceo profundo**
   >
   >
   >Las listas inteligentes pueden hacer cosas increíbles. Obtenga más información en el buceo [profundo con lista](../../product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)inteligente.

1. Busque el activador y, a continuación, arrástrelo y suéltelo en el lienzo.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Una campaña inteligente con activadores se ejecuta en el modo Activador. Funciona de una persona a la vez en función de los eventos activados y los filtros agregados.

1. Haga clic en la lista desplegable **Nombre** y seleccione un operador.

   ![](assets/smart-list-dropdown-hands.png)

1. Defina el activador.

   ![](assets/smart-lislt-select-content-hands.png)

1. Añada la restricción **Type** .

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Seleccione el origen que necesita para la lista inteligente.

   ![](assets/pc-add-constraint.png)

1. Si está utilizando el origen de correo electrónico para el contenido predictivo, agregue el activador **Clicks Link en Correo electrónico **desencadenador. Seleccione el correo electrónico y agregue la restricción **Es predictivo** , definida como **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Añada cualquier otro filtros según sea necesario.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >En una campaña inteligente con activadores y filtros, los activadores van en la parte superior. Cuando se activa, solo las personas que cumplen los criterios del filtro atraviesan el flujo.

   >[!NOTE]
   >
   >Con varios activadores, una persona pasa al flujo si ALGUNO de los activadores se activa.

   [definir una lista inteligente para una campaña inteligente por lotes](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)

   >[!NOTE]
   >
   >**Artículos relacionados**
   >
   >    
   >    
   >    * [Definir Lista inteligente para Campaña inteligente | Lote](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >    * [Añadir un paso de flujo en una Campaña inteligente](../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >    * [Definir una Lista inteligente para Actividades de personalización web](../../product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >    * [Habilitar contenido predictivo para medios enriquecidos por Web](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >    * [Habilitar la barra de recomendaciones de contenido](enabling-predictive-content/enable-the-content-recommendation-bar.md)


Para ejecutar la campaña en un grupo de personas al mismo tiempo, aprenda a .