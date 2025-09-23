---
unique-page-id: 7513680
description: Automatización de una alerta para posibles usuarios duplicados - Documentos de Marketo - Documentación del producto
title: Automatización de una alerta para posibles usuarios duplicados
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 9%

---

# Automatización de una alerta para posibles usuarios duplicados {#automate-an-alert-for-possible-duplicate-people}

¿Desea recibir una alerta cada vez que se cree un posible duplicado? A continuación se indica cómo configurar una campaña inteligente para hacerlo.

1. [Crear una nueva campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Defina la siguiente lista inteligente:

* Déclencheur: **[!UICONTROL Se ha creado la persona]**
* Filtro: **[!UICONTROL Campos duplicados]**. El nombre de campo **[!UICONTROL es] [!UICONTROL Nombre completo]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Sé creativo. Experimente con diferentes campos para obtener mejores resultados de filtrado.

1. En el paso de flujo, elija [[!UICONTROL Enviar alerta]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} acción de flujo.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Usando [Enviar token de información de alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} para incluir un vínculo a la persona en su CRM.

   >[!CAUTION]
   >
   >Si importa una lista grande, puede recibir muchas de estas alertas de una sola vez.
   >
   >Además, dos personas con el mismo nombre no significa automáticamente que sean la misma persona.

1. Active la campaña en la ficha **[!UICONTROL Programar]**.

   ![](assets/automate-an-alert-3.png)

¡Ya está! Esta campaña inteligente entrará en déclencheur cada vez que se cree una nueva persona con un nombre completo existente en Marketo.

>[!MORELIKETHIS]
>
>[Buscar y combinar personas duplicadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
