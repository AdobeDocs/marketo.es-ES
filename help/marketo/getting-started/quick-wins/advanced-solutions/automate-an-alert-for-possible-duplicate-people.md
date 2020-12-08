---
unique-page-id: 7513680
description: Automatizar una alerta para posibles Duplicados - Documentos de marketing - Documentación del producto
title: Automatizar una alerta para posibles personas Duplicados
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Automatizar una alerta para posibles personas Duplicados {#automate-an-alert-for-possible-duplicate-people}

¿Desea una alerta cada vez que se cree una persona de duplicado posible? A continuación se muestra cómo configurar una Campaña inteligente para hacerlo.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. [Cree una nueva campaña](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)inteligente. Defina la siguiente lista inteligente:

   * Activador: **Persona creada**
   * Filtro: **Campos de Duplicado. **Nombre de campo **es** Nombre **** completo.

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Sé creativo. Experimente con diferentes campos para obtener mejores resultados de filtrado.

1. En el paso de flujo, elija [Enviar acción de flujo de alerta](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) .

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Uso del token [](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Enviar información de alerta para incluir un vínculo a la persona en su CRM.

   >[!CAUTION]
   >
   >Si importa una gran lista, puede que reciba un montón de estas alertas a la vez.
   >
   >
   >Además, dos personas con el mismo nombre no significa automáticamente que sean la misma persona.

1. Active la campaña en la ficha **Programación** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

¡Eso es todo! Esta campaña inteligente se activará cada vez que se cree una nueva persona con un nombre completo existente en Marketing.

>[!MORELIKETHIS]
>
>* [Buscar y combinar personas de Duplicado](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

