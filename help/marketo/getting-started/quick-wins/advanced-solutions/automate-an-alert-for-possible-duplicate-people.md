---
unique-page-id: 7513680
description: 'Automatizar una alerta para posibles personas duplicadas: Documentos de Marketo: Documentación del producto'
title: Automatizar una alerta para posibles personas duplicadas
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Automatizar una alerta para posibles personas duplicadas {#automate-an-alert-for-possible-duplicate-people}

¿Desea crear una alerta cada vez que se cree una persona duplicada? A continuación se muestra cómo configurar una campaña inteligente para hacerlo.

1. [Cree una nueva campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md). Defina la siguiente lista inteligente:

* Déclencheur: **La persona es creada**
* Filtro: **Campos duplicados.** Nombre de campo  **es Nombre completo**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Sé creativo. Experimente con diferentes campos para obtener mejores resultados de filtrado.

1. En el paso de flujo, seleccione la acción de flujo [Send Alert](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md).

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Usar el [Send Alert Info token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) para incluir un vínculo a la persona en el CRM.

   >[!CAUTION]
   >
   >Si importa una lista grande, puede obtener un montón de estas alertas a la vez.
   >
   >Además, dos personas con el mismo nombre no significa automáticamente que sean la misma persona.

1. Active la campaña en la pestaña **Schedule**.

   ![](assets/image2017-3-27-8-3a24-3a37.png)

¡Eso es todo! Esta campaña inteligente se déclencheur cada vez que se cree una nueva persona con un nombre completo existente en Marketo.

>[!MORELIKETHIS]
>
>[Buscar y combinar personas duplicadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
