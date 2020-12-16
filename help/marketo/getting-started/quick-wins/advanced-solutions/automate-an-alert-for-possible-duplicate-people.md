---
unique-page-id: 7513680
description: Automatizar una alerta para posibles Duplicados - Documentos de marketing - Documentación del producto
title: Automatizar una alerta para posibles personas Duplicados
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Automatizar una alerta para posibles personas Duplicados {#automate-an-alert-for-possible-duplicate-people}

¿Desea una alerta cada vez que se cree una persona de duplicado posible? A continuación se muestra cómo configurar una Campaña inteligente para hacerlo.

1. [Cree una nueva campaña](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)inteligente. Defina la siguiente lista inteligente:

* Activador: **Persona creada**
* Filtro: **Campos de duplicado.** El nombre del campo **es el nombre completo**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Sé creativo. Experimente con diferentes campos para obtener mejores resultados de filtrado.

1. En el paso de flujo, elija [Enviar acción de flujo de alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) .

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Uso del token [](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Enviar información de alerta para incluir un vínculo a la persona en su CRM.

   >[!CAUTION]
   >
   >Si importa una gran lista, puede que reciba un montón de estas alertas a la vez.
   >
   >Además, dos personas con el mismo nombre no significa automáticamente que sean la misma persona.

1. Active la campaña en la ficha **Programación** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

¡Eso es todo! Esta campaña inteligente se activará cada vez que se cree una nueva persona con un nombre completo existente en Marketing.

>[!MORELIKETHIS]
>
>[Buscar y combinar personas de Duplicado](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
